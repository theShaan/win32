---
title: ImportRetailPurchaseLicenseKeyPack method of the Win32_TSLicenseKeyPack class
description: Imports, from another Remote Desktop license server, a Remote Desktop Services license key pack that was purchased through a retail channel.
ms.assetid: B45C3263-216E-4284-89A1-BE2ADE3A8E84
ms.tgt_platform: multiple
keywords:
- ImportRetailPurchaseLicenseKeyPack method Remote Desktop Services
- ImportRetailPurchaseLicenseKeyPack method Remote Desktop Services , Win32_TSLicenseKeyPack class
- Win32_TSLicenseKeyPack class Remote Desktop Services , ImportRetailPurchaseLicenseKeyPack method
topic_type:
- apiref
api_name:
- Win32_TSLicenseKeyPack.ImportRetailPurchaseLicenseKeyPack
api_location:
- TlsWmiProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
---

# ImportRetailPurchaseLicenseKeyPack method of the Win32\_TSLicenseKeyPack class

Imports, from another Remote Desktop license server, a Remote Desktop Services license key pack that was purchased through a retail channel.

## Syntax


```mof
uint32 ImportRetailPurchaseLicenseKeyPack(
  [in]  string sLicenseCode,
  [in]  string sSourceLSName,
  [in]  string sSourceLSProductId,
  [out] uint32 KeyPackId
);
```



## Parameters

<dl> <dt>

*sLicenseCode* \[in\]
</dt> <dd>

Contains the 25-character license code. Only the 25-character alphanumeric character string should be given as input. No hyphens should be added.

</dd> <dt>

*sSourceLSName* \[in\]
</dt> <dd>

The name of the source Remote Desktop license server. This is either the fully qualified distinguished name or the IP address of the server.

</dd> <dt>

*sSourceLSProductId* \[in\]
</dt> <dd>

The Remote Desktop license server identifier. The is a 35-character alphanumeric string that cannot include hyphens.

</dd> <dt>

*KeyPackId* \[out\]
</dt> <dd>

Receives the key pack identifier.

</dd> </dl>

## Return value

If the method succeeds, it returns zero. If the method is unsuccessful, it returns a nonzero value. For a list of error codes, see [Remote Desktop Services WMI Provider Error Codes](terminal-services-wmi-provider-error-codes.md).

## Requirements



| Requirement | Value |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                 |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                            |
| Namespace<br/>                | Root\\CIMv2<br/>                                                                    |
| MOF<br/>                      | <dl> <dt>TlsWmiProv.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TlsWmiProv.dll</dt> </dl> |



## See also

<dl> <dt>

[**Win32\_TSLicenseKeyPack**](win32-tslicensekeypack.md)
</dt> </dl>

 

 





