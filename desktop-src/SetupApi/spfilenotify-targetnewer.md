---
Description: The SPFILENOTIFY\_TARGETNEWER notification is sent to the callback routine if the file to be copied was queued with the SP\_COPY\_NEWER or SP\_COPY\_FORCE\_NEWER flags specified and a newer version of the file already exists in the target directory.
ms.assetid: 93bcd610-f75d-4900-841c-f67946af5c4a
title: SPFILENOTIFY_TARGETNEWER message (Setupapi.h)
ms.topic: reference
ms.date: 05/31/2018
---

# SPFILENOTIFY\_TARGETNEWER message

The **SPFILENOTIFY\_TARGETNEWER** notification is sent to the callback routine if the file to be copied was queued with the SP\_COPY\_NEWER or SP\_COPY\_FORCE\_NEWER flags specified and a newer version of the file already exists in the target directory. It can be sent to the callback routine alone or ORed together with [**SPFILENOTIFY\_LANGMISMATCH**](spfilenotify-langmismatch.md) and/or [**SPFILENOTIFY\_TARGETEXISTS**](spfilenotify-targetexists.md).


```C++
SPFILENOTIFY_TARGETNEWER
  Param1 = (UINT) FilePathInfo;
  Param2 = (UINT) 0;
            
```



## Parameters

<dl> <dt>

*Param1* 
</dt> <dd>

Pointer to a [**FILEPATHS**](/windows/desktop/api/Setupapi/ns-setupapi-filepaths_a) structure that contains information about the paths for source and target files.

</dd> <dt>

*Param2* 
</dt> <dd>

This parameter is not used unless this notification is combined, by using the OR operator, with [**SPFILENOTIFY\_LANGMISMATCH**](spfilenotify-langmismatch.md).

</dd> </dl>

## Return value

The callback routine should return one of the following values.



| Return code                                                                          | Description                                            |
|--------------------------------------------------------------------------------------|--------------------------------------------------------|
| <dl> <dt>**TRUE**</dt> </dl>  | Overwrite the file in the target directory.<br/> |
| <dl> <dt>**FALSE**</dt> </dl> | Skip the current copy operation.<br/>            |



 

## Requirements



| Requirement | Value |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Setupapi.h</dt> </dl> |



## See also

<dl> <dt>

[Overview](overview.md)
</dt> <dt>

[Notifications](notifications.md)
</dt> <dt>

[**FILEPATHS**](/windows/desktop/api/Setupapi/ns-setupapi-filepaths_a)
</dt> <dt>

[**SetupCommitFileQueue**](/windows/desktop/api/Setupapi/nf-setupapi-setupcommitfilequeuea)
</dt> <dt>

[**SetupDefaultQueueCallback**](/windows/desktop/api/Setupapi/nf-setupapi-setupdefaultqueuecallbacka)
</dt> <dt>

[**SetupInstallFile**](/windows/desktop/api/Setupapi/nf-setupapi-setupinstallfilea)
</dt> <dt>

[**SetupInstallFileEx**](/windows/desktop/api/Setupapi/nf-setupapi-setupinstallfileexa)
</dt> <dt>

[**SetupInstallFromInfSection**](/windows/desktop/api/Setupapi/nf-setupapi-setupinstallfrominfsectiona)
</dt> </dl>

 

 




