---
title: "Multiple Targets | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-tools"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
helpviewer_keywords: ["makefiles, targets", "multiple targets in NMAKE", "targets, multiple in NMAKE", "NMAKE program, targets"]
ms.assetid: b609a179-0b9f-4b08-9930-998047588ae0
caps.latest.revision: 10
author: "corob-msft"
ms.author: "corob"
manager: "ghogen"
---
# Multiple Targets
NMAKE evaluates multiple targets in a single dependency as if each were specified in a separate description block.  
  
 For example, this...  
  
```Output  
bounce.exe leap.exe : jump.obj  
   echo Building...  
```  
  
 ...is evaluated as this:  
  
```Output  
bounce.exe : jump.obj  
   echo Building...  
leap.exe : jump.obj  
   echo Building...  
```  
  
## See Also  
 [Targets](../build/targets.md)