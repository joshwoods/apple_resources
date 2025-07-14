

- UIKit
- UISceneError
-  UISceneError.Code 

Enumeration

# UISceneError.Code

Error codes for issues with scenes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case multipleScenesNotSupported

An error that indicates multiple scenes aren’t supported.

case requestDenied

An error that indicates the request was denied.

case geometryRequestUnsupported

An error that indicates the geometry request is invalid or unsupported.

case geometryRequestDenied

An error that indicates the geometry request is valid but the system denied the request.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct UISceneError

Errors returned during the creation or management of a scene.

let UISceneErrorDomain: String

The domain for scene-related errors.

