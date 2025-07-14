

- Security
-  SecCodeSignatureFlags 

Structure

# SecCodeSignatureFlags

Specify option flags that can be embedded in a code signature during signing and that govern the use of the signature.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecCodeSignatureFlags
```

## Overview

Some of these flags can be set through the `codesign(1)` command’s `--options` argument and some are set implicitly based on signing circumstances. The flags here appear as the value associated with the kSecCodeInfoFlags key in the signing information dictionary. See Signing Information Dictionary Keys.

## Topics

### Initializers

init(rawValue: UInt32)

### Constants

static var host: SecCodeSignatureFlags

May host guest code.

static var adhoc: SecCodeSignatureFlags

Must be used without a signing identity.

static var forceHard: SecCodeSignatureFlags

Always set the hard status flag on launch.

static var forceKill: SecCodeSignatureFlags

Always set the termination status flag on launch.

static var forceExpiration: SecCodeSignatureFlags

Always set the considerExpiration flag when validating the code.

static var enforcement: SecCodeSignatureFlags

Enforce code signing.

static var libraryValidation: SecCodeSignatureFlags

Require library validation.

static var restrict: SecCodeSignatureFlags

Restrict dyld loading.

static var runtime: SecCodeSignatureFlags

Apply runtime hardening policies as required by the hardened runtime version.

### Type Properties

static var linkerSigned: SecCodeSignatureFlags

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

