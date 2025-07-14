

- Security
- Certificate, Key, and Trust Services
- Policies
-  Revocation Policy Constants 

API Collection

# Revocation Policy Constants

Use these flags to create a revocation policy object.

## Overview

Use these flags with a call to the SecPolicyCreateRevocation(_:) function to characterize the constructed policy.

## Topics

### Constants

var kSecRevocationCRLMethod: CFOptionFlags

Perform revocation checking using the CRL (Certification Revocation List) method.

var kSecRevocationNetworkAccessDisabled: CFOptionFlags

Consult only locally cached replies; do not use network access.

var kSecRevocationOCSPMethod: CFOptionFlags

Perform revocation checking using OCSP (Online Certificate Status Protocol).

var kSecRevocationPreferCRL: CFOptionFlags

Prefer CRL revocation checking over OCSP; by default, OCSP is preferred.

var kSecRevocationRequirePositiveResponse: CFOptionFlags

Require a positive response to pass the policy.

var kSecRevocationUseAnyAvailableMethod: CFOptionFlags

Perform either OCSP or CRL checking.

