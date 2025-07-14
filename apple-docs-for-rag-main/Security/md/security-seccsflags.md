

- Security
-  SecCSFlags 

Structure

# SecCSFlags

Values that can be used in the `flags` parameter to most code signing functions.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecCSFlags
```

## Overview

All of the bits in the SecCSFlags enumeration are reserved by Apple. If you set any bits not defined here, the behavior is undefined.

## Topics

### Initializers

init(rawValue: UInt32)

### Constants

static var considerExpiration: SecCSFlags

Consider expired certificates invalid.

static var enforceRevocationChecks: SecCSFlags

static var checkTrustedAnchors: SecCSFlags

static var noNetworkAccess: SecCSFlags

static var reportProgress: SecCSFlags

static var quickCheck: SecCSFlags

### Type Properties

static var applyEmbeddedPolicy: SecCSFlags

static var matchGuestRequirementInKernel: SecCSFlags

static var stripDisallowedXattrs: SecCSFlags

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

