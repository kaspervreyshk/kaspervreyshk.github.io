---
title: "What Really Happens When You Click Yes"
date: 2026-02-20
draft: false
---

This post presents a detailed analysis of the Windows User Account Control elevation mechanism as implemented in Windows 11 24H2. Through kernel debugging and static reverse engineering of ntoskrnl.exe, appinfo.dll, and consent.exe, we document the full elevation pipeline from the initial ShellExecuteEx call to the creation of an unrestricted access token. We examine the role of the AppInfo service in process creation, the Secure Desktop isolation model used by consent.exe, the kernel-level token duplication and privilege adjustment routines, and the undocumented internal structures involved at each stage. All findings were reproduced on a live debug environment using WinDbg attached to a Windows 11 virtual machine over a serial connection.
