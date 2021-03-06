---
title: Examining the Stack Trace
description: Examining the Stack Trace
ms.assetid: ca203f29-841f-411e-915a-81abaa96a8e6
keywords: ["Debugger Engine API, stack trace"]
ms.author: windowsdriverdev
ms.date: 05/23/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Examining the Stack Trace


A *call stack* contains the data for the functions calls made by a thread. The data for each function call is called a *stack frame* and includes the return address, parameters passed to the function, and the function's local variables. Each time a function call is made a new stack frame is pushed onto the top of the stack. When that function returns, the stack frame is popped off the stack.

Each thread has its own call stack, representing the calls made in that thread.

To get a stack trace, use the methods [**GetStackTrace**](https://msdn.microsoft.com/library/windows/hardware/ff548425) and [**GetContextStackTrace**](https://msdn.microsoft.com/library/windows/hardware/ff545748). A stack trace can be printed using [**OutputStackTrace**](https://msdn.microsoft.com/library/windows/hardware/ff553252) and [**OutputContextStackTrace**](https://msdn.microsoft.com/library/windows/hardware/ff553203).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[debugger\debugger]:%20Examining%20the%20Stack%20Trace%20%20RELEASE:%20%285/15/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




