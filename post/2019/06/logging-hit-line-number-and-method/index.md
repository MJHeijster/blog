---
title: "Logging hit line number and method"
date: "2019-06-20"
categories: 
  - "tutorial"
tags: 
  - "hit"
  - "line"
  - "logging"
  - "method"
  - "number"
coverImage: "artificial-intelligence-blur-close-up-546819.jpg"
---

During debugging I had issues figuring out where my code just stopped. Since I had no debugging methods on that server, I wanted to create a better way of logging than int count=0;Console.WriteLine(count++);

While looking for a way of logging the line number I found the [CompilerServices](https://docs.microsoft.com/en-us/dotnet/api/system.runtime.compilerservices?view=netframework-4.8) namespace which has a [CallerLineNumber](https://docs.microsoft.com/en-us/dotnet/api/system.runtime.compilerservices.callerlinenumberattribute?view=netframework-4.8) and [CallerMemberName](https://docs.microsoft.com/en-us/dotnet/api/system.runtime.compilerservices.callermembernameattribute?view=netframework-4.8).

Using that, I made this small method to log the method and line number:

`private void LogLineNumber([System.Runtime.CompilerServices.CallerLineNumber] int lineNumber = 0, [System.Runtime.CompilerServices.CallerMemberName] string caller = null) { Console.WriteLine($"Hit line number {lineNumber} for {caller}."); }`
