

- Security
- Certificate, Key, and Trust Services
- Trust
-  Discovering Why a Trust Evaluation Failed 

Article

# Discovering Why a Trust Evaluation Failed

Determine whether you can recover from a failed trust evaluation.

## Overview

Many factors affect the outcome of a trust evaluation. These include whether the system can locate all of the intermediate certificates, the validity of the certificates in the chain, and the characteristics of the certificates. Some issues, like a revoked certificate, result in an absolute failure and should *not* be circumvented. In other cases, you might get a different result by changing the conditions of the evaluation. For example, an expired certificate might have been valid when the corresponding identity was used to sign a document.

To get the specific reason for trust failure, examine the error parameter provided in the evaluation callback described in Evaluating a Trust and Parsing the Result. The error’s code indicates the reason, or in the case of multiple errors, the most serious reason for the failure. For example, a revoked certificate results in an error with the code errSecCertificateRevoked, while an expired certificate produces errSecCertificateExpired.

To determine whether the system considers the failure recoverable, use the SecTrustGetTrustResult(_:_:) method.

- Swift
- Objective-C

```
var trustResult = SecTrustResultType.invalid
SecTrustGetTrustResult(trust, &trustResult)
if trustResult == .recoverableTrustFailure {
    // Make changes and try again.
}
```

```
SecTrustResultType trustResult;
SecTrustGetTrustResult(trust, &trustResult);
if (trustResult == kSecTrustResultRecoverableTrustFailure) {
    // Make changes and try again.
}
```

For a result of SecTrustResultType.recoverableTrustFailure, and based on the error you receive, you may be able to remedy problems by reconfiguring and reevaluating the trust, as described in Configuring a Trust.

