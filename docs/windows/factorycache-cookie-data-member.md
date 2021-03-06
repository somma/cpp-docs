---
title: "FactoryCache::cookie Data Member | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-windows"]
ms.tgt_pltfrm: ""
ms.topic: "reference"
f1_keywords: ["module/Microsoft::WRL::Details::FactoryCache::cookie"]
dev_langs: ["C++"]
helpviewer_keywords: ["cookie data member"]
ms.assetid: b1bc79af-a896-4e3b-8afa-64733022eddf
caps.latest.revision: 7
author: "mikeblome"
ms.author: "mblome"
manager: "ghogen"
---
# FactoryCache::cookie Data Member
Supports the Windows Runtime C++ Template Library infrastructure and is not intended to be used directly from your code.  
  
## Syntax  
  
```  
union {   
   WINRT_REGISTRATION_COOKIE winrt;  
   DWORD com;   
} cookie;  
```  
  
## Remarks  
 Contains a value that identifies a registered Windows Runtime or COM class object, and is later used to unregister the object.  
  
## Requirements  
 **Header:** module.h  
  
 **Namespace:** Microsoft::WRL::Details  
  
## See Also  
 [FactoryCache Structure](../windows/factorycache-structure.md)   
 [Microsoft::WRL::Details Namespace](../windows/microsoft-wrl-details-namespace.md)