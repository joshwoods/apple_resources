

- Combine
- ObservableObject
-  objectWillChange 

Instance Property

# objectWillChange

A publisher that emits before the object has changed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var objectWillChange: Self.ObjectWillChangePublisher { get }
```

**Required** Default implementation provided.

## Default Implementations

### ObservableObject Implementations

var objectWillChange: ObservableObjectPublisher

## See Also

### Publishing Changes

associatedtype ObjectWillChangePublisher : Publisher = ObservableObjectPublisher

The type of publisher that emits before the object has changed.

**Required**

