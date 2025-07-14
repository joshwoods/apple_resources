

- Security
- Certificate, Key, and Trust Services
- Policies
-  Security Policy Keys 

API Collection

# Security Policy Keys

Use these dictionary keys to get and set policy properties.

## Overview

Use these keys with calls to the SecPolicyCopyProperties(_:) and SecPolicySetProperties functions.

## Topics

### Constants

let kSecPolicyOid: CFString

The object identifier that defines the policy type (`CFStringRef`). All policies have a value for this key.

let kSecPolicyName: CFString

A name (`CFStringRef`) that the certificate must match to satisfy this policy. For SSL/TLS, this specifies the server name which must match the common name of the certificate. For S/MIME, this specifies the RFC 822 email address.

let kSecPolicyClient: CFString

If true, indicates this policy should be evaluated against the client certificate. If false, the policy is evaluated against the certificate for the server. Default is false.

let kSecPolicyRevocationFlags: CFString

let kSecPolicyTeamIdentifier: CFString

let kSecPolicyKU_DigitalSignature: CFString

If true, the certificate’s key usage must allow it to be used for signing.

let kSecPolicyKU_NonRepudiation: CFString

If true, the certificate’s key usage must allow it to be used for non-repudiation.

let kSecPolicyKU_KeyEncipherment: CFString

If true, the certificate’s key usage must allow it to be used for key encryption.

let kSecPolicyKU_DataEncipherment: CFString

If true, the certificate’s key usage must allow it to be used for data encryption.

let kSecPolicyKU_KeyAgreement: CFString

If true, the certificate’s key usage must allow it to be used for key agreement.

let kSecPolicyKU_KeyCertSign: CFString

If true, the certificate’s key usage must allow it to be used for signing certificates.

let kSecPolicyKU_CRLSign: CFString

If true, the certificate’s key usage must allow it to be used for signing certificate revocation lists (CRLs).

let kSecPolicyKU_EncipherOnly: CFString

If true, the certificate’s key usage must allow it to be used *only* for encryption.

let kSecPolicyKU_DecipherOnly: CFString

If true, the certificate’s key usage must allow it to be used *only* for decryption.

