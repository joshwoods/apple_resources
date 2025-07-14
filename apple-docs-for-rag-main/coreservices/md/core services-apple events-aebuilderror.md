

- Core Services
- Apple Events
-  AEBuildError 

Structure

# AEBuildError

Defines a structure for storing additional error codeinformation for “AEBuild” routines.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AEBuildError
```

## Topics

### Initializers

init()

init(fError: AEBuildErrorCode, fErrorPos: UInt32)

### Instance Properties

var fError: AEBuildErrorCode

The error code. See AEBuildErrorCode for alist of errors.

var fErrorPos: UInt32

The character position where the parser detectedthe error.

