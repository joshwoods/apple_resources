

- Combine
- Subscribers
- Subscribers.Assign
-  object 

Instance Property

# object

The object that contains the property to assign.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final var object: Root? { get }
```

## Discussion

The subscriber holds a strong reference to this object until the upstream publisher calls receive(completion:), at which point the subscriber sets this property to `nil`.

## See Also

### Inspecting the Assigned Property

let keyPath: ReferenceWritableKeyPath&lt;Root, Input>

The key path that indicates the property to assign.

