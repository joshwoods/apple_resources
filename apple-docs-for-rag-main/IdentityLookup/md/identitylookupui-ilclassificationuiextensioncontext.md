

- IdentityLookupUI
-  ILClassificationUIExtensionContext 

Class

# ILClassificationUIExtensionContext

An object that manages the state of the current request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILClassificationUIExtensionContext
```

## Topics

### Readying the Response

var isReadyForClassificationResponse: Bool

A Boolean value that determines whether the extension has enough information to complete the report.

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing the Request

var extensionContext: ILClassificationUIExtensionContext

The context for the current request.

