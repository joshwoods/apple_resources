

- Security
-  SecTrustResultType 

Enumeration

# SecTrustResultType

Trust evaluation result codes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SecTrustResultType
```

## Overview

You get one of these constants when you call the SecTrustGetTrustResult(_:_:) method after evaluating a trust instance with either the SecTrustEvaluateWithError(_:_:) method or the SecTrustEvaluateAsyncWithError(_:_:_:) method. If evaluation fails and SecTrustGetTrustResult(_:_:) reports SecTrustResultType.recoverableTrustFailure, you might be able to change parameters like the evaluation date, and reevaluate to obtain a passing result, as described in Configuring a Trust.

See an individual constant below for more information about how to handle that result type in your app.

## Topics

### Result Codes

case unspecified

The user did not specify a trust setting.

case proceed

The user granted permission to trust the certificate for the purposes designated in the specified policies.

case deny

The user specified that the certificate should not be trusted.

case recoverableTrustFailure

Trust is denied, but recovery may be possible.

case fatalTrustFailure

Trust is denied and no simple fix is available.

case otherError

A value that indicates a failure other than trust evaluation.

case invalid

An indication of an invalid setting or result.

case confirm

User confirmation is required before proceeding.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

