

- Security
- Certificate, Key, and Trust Services
- Certificates
-  Certificate OIDs 

API Collection

# Certificate OIDs

Use OIDs as keys in the dictionary representing certificate values.

## Overview

These Object Identifiers (OIDs) are the keys that may appear in the dictionary returned by a call to the SecCertificateCopyValues(_:_:_:) function. The values associated with these keys are themselves dictionaries that represent the given property of a certificate, and that may have the keys listed in Certificate Property Keys.

## Topics

### Constants

let kSecOIDADC_CERT_POLICY: CFString

let kSecOIDAPPLE_CERT_POLICY: CFString

let kSecOIDAPPLE_EKU_CODE_SIGNING: CFString

let kSecOIDAPPLE_EKU_CODE_SIGNING_DEV: CFString

let kSecOIDAPPLE_EKU_ICHAT_ENCRYPTION: CFString

let kSecOIDAPPLE_EKU_ICHAT_SIGNING: CFString

let kSecOIDAPPLE_EKU_RESOURCE_SIGNING: CFString

let kSecOIDAPPLE_EKU_SYSTEM_IDENTITY: CFString

let kSecOIDAPPLE_EXTENSION: CFString

let kSecOIDAPPLE_EXTENSION_AAI_INTERMEDIATE: CFString

let kSecOIDAPPLE_EXTENSION_ADC_APPLE_SIGNING: CFString

let kSecOIDAPPLE_EXTENSION_ADC_DEV_SIGNING: CFString

let kSecOIDAPPLE_EXTENSION_APPLEID_INTERMEDIATE: CFString

let kSecOIDAPPLE_EXTENSION_APPLE_SIGNING: CFString

let kSecOIDAPPLE_EXTENSION_CODE_SIGNING: CFString

let kSecOIDAPPLE_EXTENSION_INTERMEDIATE_MARKER: CFString

let kSecOIDAPPLE_EXTENSION_ITMS_INTERMEDIATE: CFString

let kSecOIDAPPLE_EXTENSION_WWDR_INTERMEDIATE: CFString

let kSecOIDAuthorityInfoAccess: CFString

let kSecOIDAuthorityKeyIdentifier: CFString

let kSecOIDBasicConstraints: CFString

let kSecOIDBiometricInfo: CFString

let kSecOIDCSSMKeyStruct: CFString

let kSecOIDCertIssuer: CFString

let kSecOIDCertificatePolicies: CFString

let kSecOIDClientAuth: CFString

let kSecOIDCollectiveStateProvinceName: CFString

let kSecOIDCollectiveStreetAddress: CFString

let kSecOIDCommonName: CFString

let kSecOIDCountryName: CFString

let kSecOIDCrlDistributionPoints: CFString

let kSecOIDCrlNumber: CFString

let kSecOIDCrlReason: CFString

let kSecOIDDOTMAC_CERT_EMAIL_ENCRYPT: CFString

let kSecOIDDOTMAC_CERT_EMAIL_SIGN: CFString

let kSecOIDDOTMAC_CERT_EXTENSION: CFString

let kSecOIDDOTMAC_CERT_IDENTITY: CFString

let kSecOIDDOTMAC_CERT_POLICY: CFString

let kSecOIDDeltaCrlIndicator: CFString

let kSecOIDDescription: CFString

let kSecOIDEKU_IPSec: CFString

let kSecOIDEmailAddress: CFString

let kSecOIDEmailProtection: CFString

let kSecOIDExtendedKeyUsage: CFString

let kSecOIDExtendedKeyUsageAny: CFString

let kSecOIDExtendedUseCodeSigning: CFString

let kSecOIDGivenName: CFString

let kSecOIDHoldInstructionCode: CFString

let kSecOIDInvalidityDate: CFString

let kSecOIDIssuerAltName: CFString

let kSecOIDIssuingDistributionPoint: CFString

let kSecOIDIssuingDistributionPoints: CFString

let kSecOIDKERBv5_PKINIT_KP_CLIENT_AUTH: CFString

let kSecOIDKERBv5_PKINIT_KP_KDC: CFString

let kSecOIDKeyUsage: CFString

let kSecOIDLocalityName: CFString

let kSecOIDMS_NTPrincipalName: CFString

let kSecOIDMicrosoftSGC: CFString

let kSecOIDNameConstraints: CFString

let kSecOIDNetscapeCertSequence: CFString

let kSecOIDNetscapeCertType: CFString

let kSecOIDNetscapeSGC: CFString

let kSecOIDOCSPSigning: CFString

let kSecOIDOrganizationName: CFString

let kSecOIDOrganizationalUnitName: CFString

let kSecOIDPolicyConstraints: CFString

let kSecOIDPolicyMappings: CFString

let kSecOIDPrivateKeyUsagePeriod: CFString

let kSecOIDQC_Statements: CFString

let kSecOIDSRVName: CFString

let kSecOIDSerialNumber: CFString

let kSecOIDServerAuth: CFString

let kSecOIDStateProvinceName: CFString

let kSecOIDStreetAddress: CFString

let kSecOIDSubjectAltName: CFString

let kSecOIDSubjectDirectoryAttributes: CFString

let kSecOIDSubjectEmailAddress: CFString

let kSecOIDSubjectInfoAccess: CFString

let kSecOIDSubjectKeyIdentifier: CFString

let kSecOIDSubjectPicture: CFString

let kSecOIDSubjectSignatureBitmap: CFString

let kSecOIDSurname: CFString

let kSecOIDTimeStamping: CFString

let kSecOIDTitle: CFString

let kSecOIDUseExemptions: CFString

let kSecOIDX509V1CertificateIssuerUniqueId: CFString

let kSecOIDX509V1CertificateSubjectUniqueId: CFString

let kSecOIDX509V1IssuerName: CFString

let kSecOIDX509V1IssuerNameCStruct: CFString

let kSecOIDX509V1IssuerNameLDAP: CFString

let kSecOIDX509V1IssuerNameStd: CFString

let kSecOIDX509V1SerialNumber: CFString

let kSecOIDX509V1Signature: CFString

let kSecOIDX509V1SignatureAlgorithm: CFString

let kSecOIDX509V1SignatureAlgorithmParameters: CFString

let kSecOIDX509V1SignatureAlgorithmTBS: CFString

let kSecOIDX509V1SignatureCStruct: CFString

let kSecOIDX509V1SignatureStruct: CFString

let kSecOIDX509V1SubjectName: CFString

let kSecOIDX509V1SubjectNameCStruct: CFString

let kSecOIDX509V1SubjectNameLDAP: CFString

let kSecOIDX509V1SubjectNameStd: CFString

let kSecOIDX509V1SubjectPublicKey: CFString

let kSecOIDX509V1SubjectPublicKeyAlgorithm: CFString

let kSecOIDX509V1SubjectPublicKeyAlgorithmParameters: CFString

let kSecOIDX509V1SubjectPublicKeyCStruct: CFString

let kSecOIDX509V1ValidityNotAfter: CFString

let kSecOIDX509V1ValidityNotBefore: CFString

let kSecOIDX509V1Version: CFString

let kSecOIDX509V3Certificate: CFString

let kSecOIDX509V3CertificateCStruct: CFString

let kSecOIDX509V3CertificateExtensionCStruct: CFString

let kSecOIDX509V3CertificateExtensionCritical: CFString

let kSecOIDX509V3CertificateExtensionId: CFString

let kSecOIDX509V3CertificateExtensionStruct: CFString

let kSecOIDX509V3CertificateExtensionType: CFString

let kSecOIDX509V3CertificateExtensionValue: CFString

let kSecOIDX509V3CertificateExtensionsCStruct: CFString

let kSecOIDX509V3CertificateExtensionsStruct: CFString

let kSecOIDX509V3CertificateNumberOfExtensions: CFString

let kSecOIDX509V3SignedCertificate: CFString

let kSecOIDX509V3SignedCertificateCStruct: CFString

