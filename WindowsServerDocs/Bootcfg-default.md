---
title: Bootcfg default
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: e21824d7-8278-41d7-a2c5-ce09803d513a
author: jaimeo
---
# Bootcfg default
Specifies the operating system entry to designate as the default.  
  
For examples of how this command can be used, see [Examples](#BKMK_examples).  
  
## Syntax  
  
```  
bootcfg /default [/s <Computer> [/u <Domain>\<User> /p <Password>]] [/id <OSEntryLineNum>]  
```  
  
## Parameters  
  
|Parameter|Description|  
|-------------|---------------|  
|\/s <Computer>|Specifies the name or IP address of a remote computer \(do not use backslashes\). The default is the local computer.|  
|\/u <Domain>\\<User>|Runs the command with the account permissions of the user specified by <User> or <Domain>\\<User>. The default is the permissions of the current logged on user on the computer issuing the command.|  
|\/p <Password>|Specifies the password of the user account that is specified in the **\/u** parameter.|  
|\/id <OSEntryLineNum>|Specifies the operating system entry line number in the \[operating systems\] section of the Boot.ini file to designate as default. The first line after the \[operating systems\] section header is 1.|  
|\/?|Displays help at the command prompt.|  
  
## <a name="BKMK_examples"></a>Examples  
The following examples show how you can use the **bootcfg \/default**command:  
  
```  
bootcfg /default /id 2  
bootcfg /default /s srvmain /u maindom\hiropln /p p@ssW23 /id 2  
```  
  
#### Additional references  
[Command-Line Syntax Key](Command-Line-Syntax-Key.md)  
  
