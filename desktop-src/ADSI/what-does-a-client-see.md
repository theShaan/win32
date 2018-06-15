---
title: What Does a Client See
description: This topic lists ways that a client views ADSI data.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\mbaldwin
ms.assetid: 238eeea9-1303-4d37-bf09-ad03f1790c1b
ms.prod: windows-server-dev
ms.technology: active-directory-domain-services
ms.tgt_platform: multiple
keywords:
- extensions ADSI ,what does a client see
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# What Does a Client See?

-   A client sees ADSI and all of its extension objects as one object.
-   An ADSI client sees one [**IDispatch**](https://msdn.microsoft.com/en-us/library/ms221608(v=VS.71).aspx) interface that handles all the dual and dispatch interfaces in the object, whether the dual or dispatch interface is implemented by the aggregator in the provider or by an extension. Please see [Resolution of Function/Property Name Conflicts in Automation in Extensions](resolution-of-functionproperty-name-conflicts-in-automation-in-extensions.md).
-   ADSI does not expose any type information through the [**IDispatch::GetTypeInfo**](https://msdn.microsoft.com/en-us/library/ms221571(v=VS.71).aspx) or [**IDispatch::GetTypeInfoCount**](https://msdn.microsoft.com/en-us/library/ms221674(v=VS.71).aspx) methods. ADSI provides type information through the type library.

 

 



