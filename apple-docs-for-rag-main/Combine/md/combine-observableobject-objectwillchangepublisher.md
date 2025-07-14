

- Combine
- ObservableObject
-  ObjectWillChangePublisher 

Associated Type

# ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype ObjectWillChangePublisher : Publisher = ObservableObjectPublisher where Self.ObjectWillChangePublisher.Failure == Never
```

**Required**

## See Also

### Publishing Changes

var objectWillChange: Self.ObjectWillChangePublisher

A publisher that emits before the object has changed.

**Required** Default implementation provided.

