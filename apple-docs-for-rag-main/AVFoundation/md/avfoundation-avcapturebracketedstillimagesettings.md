

- AVFoundation
-  AVCaptureBracketedStillImageSettings 

Class

# AVCaptureBracketedStillImageSettings

The abstract superclass for bracketed photo capture settings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureBracketedStillImageSettings
```

## Overview

Note

The `AVCaptureBracketedStillImageSettings` class must not be instantiated directly. You should create instances of the `AVCaptureManualExposureBracketedStillImageSettings` and `AVCaptureAutoExposureBracketedStillImageSettings` classes as appropriate.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptureAutoExposureBracketedStillImageSettings
- AVCaptureManualExposureBracketedStillImageSettings

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Bracketed Settings Types

class AVCaptureAutoExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of bias relative to automatic exposure.

class AVCaptureManualExposureBracketedStillImageSettings

A configuration for defining bracketed photo captures in terms of specific exposure and ISO values.

