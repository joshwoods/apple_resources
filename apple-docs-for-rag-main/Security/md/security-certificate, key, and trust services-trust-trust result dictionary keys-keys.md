

- Security
- Certificate, Key, and Trust Services
- Trust
-  Trust Result Dictionary Keys 

API Collection

# Trust Result Dictionary Keys

Recognize the keys that appear in a dictionary containing information about an evaluated certification chain.

## Overview

These keys appear in the dictionary returned from a call to the SecTrustCopyResult(_:) function and provide information about the evaluated trust.

## Topics

### Constants

let kSecTrustCertificateTransparency: CFString

A key whose value is a Boolean used to indicate Certificate Transparency.

let kSecTrustCertificateTransparencyWhiteList: CFString

A key whose value is a Boolean used to indicate the chain satisfies Certificate Transparency by being on the allow list.

Deprecated

let kSecTrustEvaluationDate: CFString

A key whose value indicates the time that the trust evaluation took place.

let kSecTrustExtendedValidation: CFString

A key whose value is a Boolean used to indicate Extended Validation.

let kSecTrustOrganizationName: CFString

A key whose value is the organization name field of the subject of the leaf certificate.

let kSecTrustResultValue: CFString

A key whose value represents the trust evaluation result.

let kSecTrustRevocationChecked: CFString

A key whose value indicates the outcome of revocation checking during trust evaluation.

let kSecTrustRevocationValidUntilDate: CFString

A key whose value indicates the earliest date at which revocation information becomes stale.

