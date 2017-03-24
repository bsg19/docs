---
title: "-codepage (Visual Basic) | Microsoft Docs"
ms.custom: ""
ms.date: "2015-07-20"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "VB"
helpviewer_keywords: 
  - "/codepage compiler option [Visual Basic]"
  - "codepage compiler option [Visual Basic]"
  - "-codepage compiler option [Visual Basic]"
ms.assetid: be36ec33-6800-4505-838c-4124564f5cc9
caps.latest.revision: 17
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
---
# /codepage (Visual Basic)
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

Specifies the code page to use for all source-code files in the compilation.  
  
## Syntax  
  
```  
/codepage:id  
```  
  
## Arguments  
  
|||  
|-|-|  
|Term|Definition|  
|`id`|Required. The compiler uses the code page specified by `id` to interpret the encoding of the source files.|  
  
## Remarks  
 To compile source code saved with a specific encoding, you can use `/codepage` to specify which code page should be used. The `/codepage` option applies to all source-code files in your compilation. For more information, see [Character Encoding in the .NET Framework](../Topic/Character%20Encoding%20in%20the%20.NET%20Framework.md).  
  
 The `/codepage` option is not needed if the source-code files were saved using the current ANSI code page, Unicode, or UTF-8 with a signature. [!INCLUDE[vsprvs](../../../includes/vsprvs-md.md)] saves all source-code files with the current ANSI code page by default, unless the user specifies another encoding in the **Encoding** dialog box. [!INCLUDE[vsprvs](../../../includes/vsprvs-md.md)] uses the **Encoding** dialog box to open source-code files saved with a different code page.  
  
> [!NOTE]
>  The `/codepage` option is not available from within the [!INCLUDE[vsprvs](../../../includes/vsprvs-md.md)] development environment; it is available only when compiling from the command line.  
  
## See Also  
 [Visual Basic Command-Line Compiler](../../../visual-basic/reference/command-line-compiler/index.md)