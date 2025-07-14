

- PHASE
- PHASEError
-  invalidObject 

Type Property

# invalidObject

An error that indicates an object is invalid in a specific context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var invalidObject: PHASEError.Code { get }
```

## Discussion

The addChild(_:) function throws this error if the specified child already has a parent in the scene graph hierarchy.

## See Also

### Identifying an Error Cause

static var initializeFailed: PHASEError.Code

An error that indicates the engine failed to initialize.

