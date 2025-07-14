

- Security
-  SecTrustOptionFlags 

Structure

# SecTrustOptionFlags

The option flags used to condition a trust evaluation.

macOS 10.0+

``` source
struct SecTrustOptionFlags
```

## Overview

Use these flags in calls to the SecTrustSetOptions(_:_:) function.

## Topics

### Initializers

init(rawValue: UInt32)

Initializes a trust option flags structure.

### Flags

static var allowExpired: SecTrustOptionFlags

Allow expired certificates (except for the root certificate).

static var leafIsCA: SecTrustOptionFlags

Allow CA certificates as leaf certificates.

static var fetchIssuerFromNet: SecTrustOptionFlags

Allow network downloads of CA certificates.

static var allowExpiredRoot: SecTrustOptionFlags

Allow expired root certificates.

static var requireRevPerCert: SecTrustOptionFlags

Require a positive revocation check for each certificate.

static var useTrustSettings: SecTrustOptionFlags

Use TrustSettings instead of anchors.

static var implicitAnchors: SecTrustOptionFlags

Treat properly self-signed certificates as anchors implicitly.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

