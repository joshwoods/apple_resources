

- UIKit
-  UISceneError 

Structure

# UISceneError

Errors returned during the creation or management of a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct UISceneError
```

## Topics

### Identifying an error cause

static var multipleScenesNotSupported: UISceneError.Code

An error that indicates multiple scenes aren’t supported.

static var requestDenied: UISceneError.Code

An error that indicates the request was denied.

static var geometryRequestUnsupported: UISceneError.Code

An error that indicates the geometry request is invalid or unsupported.

static var geometryRequestDenied: UISceneError.Code

An error that indicates the geometry request is valid but the system denied the request.

enum Code

Error codes for issues with scenes.

### Inspecting error information

static var errorDomain: String

The domain for scene-related errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Error codes for issues with scenes.

let UISceneErrorDomain: String

The domain for scene-related errors.

