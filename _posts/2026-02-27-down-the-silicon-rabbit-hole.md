---
layout: post
title: "Down the Silicon Rabbit Hole, Alice Was Right"
date: 2026-02-27 19:40:00 +0100
categories: windows
---

Every security boundary in Windows exists because a transistor is either conducting or it isn't. Six transistors form a flip-flop. Sixty-four flip-flops form a register. Some of those registers decide what your CPU is allowed to do. The hypervisor watches over them through EPT violations and second-level address translation. But not everything is watched. Some structures live in pages that the hypervisor considers ordinary data. And ordinary data can be written. This is about what happens at every layer, from the silicon to the moment those protections stop mattering.

There is a certain elegance to all of this once you sit with it long enough. Most people, especially young researchers, never stop to consider how much the hardware matters. They want to understand the internals of something as complex and fascinating as Windows, but they skip the foundation. You cannot truly understand an operating system until you understand what it runs on. Every abstraction hides a physical truth.

![wonderland](/_images/wonderland.jpg)

That is why this article exists. We are going down together. And like the rabbit hole, this one does not end. In ours, we will try to find a wall, somewhere deep enough to say we pushed as far as we could. I find the Alice analogy particularly fitting when it comes to this kind of research. The deeper you go, the less the surface world makes sense, and the more the strange things you discover feel like they were always the real ones. I will let you think about that. I promise it is worth thinking about.

Do you know what silicon is. Element 14. Fourteen protons in the nucleus, fourteen electrons around it. A grey, hard, crystalline solid with a metallic luster. You will find it everywhere. In sand, in quartz, in rock. Silicon dioxide. SiO2. It makes up roughly 28 percent of the Earth's crust, second only to oxygen. In its pure form, it is a semiconductor. It does not conduct electricity well. But it does not block it either. It sits in between. And that property, that precise, quiet, in-between behavior, is what the entire chip industry is built on.
