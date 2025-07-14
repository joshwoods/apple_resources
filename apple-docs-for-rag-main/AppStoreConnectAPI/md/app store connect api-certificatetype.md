

- App Store Connect API
-  CertificateType 

Type

# CertificateType

Literal values that represent types of signing certificates.

App Store Connect API 1.1+

``` source
string CertificateType
```

## Possible Values 

`APPLE_PAY`  

`APPLE_PAY_MERCHANT_IDENTITY`  

`APPLE_PAY_PSP_IDENTITY`  

`APPLE_PAY_RSA`  

`DEVELOPER_ID_KEXT`  

`DEVELOPER_ID_KEXT_G2`  

`DEVELOPER_ID_APPLICATION`  

`DEVELOPER_ID_APPLICATION_G2`  

`DEVELOPMENT`  

`DISTRIBUTION`  

`IDENTITY_ACCESS`  

`IOS_DEVELOPMENT`  

`IOS_DISTRIBUTION`  

`MAC_APP_DISTRIBUTION`  

`MAC_INSTALLER_DISTRIBUTION`  

`MAC_APP_DEVELOPMENT`  

`PASS_TYPE_ID`  

`PASS_TYPE_ID_WITH_NFC`  

## Mentioned in 

App Store Connect API 3.7 release notes

## Discussion

- PossibleValues

  - DEVELOPER_ID_APPLICATION

  - DEVELOPER_ID_APPLICATION_G2

  - DEVELOPER_ID_KEXT

  - DEVELOPER_ID_KEXT_G2

  - DEVELOPMENT

  - DISTRIBUTION

  - IOS_DEVELOPMENT

  - IOS_DISTRIBUTION

  - MAC_APP_DEVELOPMENT

  - MAC_APP_DISTRIBUTION

  - MAC_INSTALLER_DISTRIBUTION

  - PASS_TYPE_ID_WITH_NFC

  - PASS_TYPE_ID

## See Also

### Object and data types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificatesResponse

A response that contains a list of Certificates resources.

object CertificateUpdateRequest

The request body you use to update a certificate activation status.

