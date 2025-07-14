

- Security
- Certificate, Key, and Trust Services
- Policies
-  Standard Policies for Specific Certificate Types 

API Collection

# Standard Policies for Specific Certificate Types

Use special OIDs to cause a certificate to be evaluated based on security policies specific to a given type of certificate.

## Topics

### Constants

let kSecPolicyAppleX509Basic: CFString

Basic X509-style certificate evaluation.

let kSecPolicyAppleSSL: CFString

Basic X509 plus host name verification per RFC 2818.

let kSecPolicyAppleSMIME: CFString

Basic X509 plus email address verification and `KeyUsage` enforcement per RFC 2632.

let kSecPolicyAppleEAP: CFString

Extensible Authentication Protocol. Functionally identical to SSL policy. A separate OID is provided to facilitate per-policy, per-certificate trust settings using the `SecTrust` mechanism.

let kSecPolicyAppleIPsec: CFString

Policy for use in IPsec communication. Functionally identical to SSL policy. A separate OID is provided to facilitate per-policy, per-certificate trust settings using the `SecTrust` mechanism.

let kSecPolicyApplePKINITClient: CFString

Kerberos Pkinit client certificate validation.

let kSecPolicyApplePKINITServer: CFString

Kerberos Pkinit server certificate validation.

let kSecPolicyAppleCodeSigning: CFString

Policy for use in evaluating Apple code signing certificates.

let kSecPolicyMacAppStoreReceipt: CFString

Policy for use in evaluating Mac App Store receipts.

let kSecPolicyAppleIDValidation: CFString

Policy for use in evaluating Apple ID certificates.

let kSecPolicyAppleTimeStamping: CFString

Policy that causes evaluation of the validity of the time stamp on a signature. This can be used to allow verification that a certificate was valid at the time that something was signed with that certificate even if the certificate is no longer valid.

let kSecPolicyApplePassbookSigning: CFString

let kSecPolicyApplePayIssuerEncryption: CFString

let kSecPolicyAppleRevocation: CFString

