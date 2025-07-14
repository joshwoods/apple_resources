

- Foundation
- NSItemProvider
-  registerObject(ofClass:visibility:loadHandler:) 

Instance Method

# registerObject(ofClass:visibility:loadHandler:)

Lazily adds representations of a specified object type to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@preconcurrency
func registerObject(
    ofClass: T.Type,
    visibility: NSItemProviderRepresentationVisibility,
    loadHandler: @escaping ((T?, (any Error)?) -> Void) -> Progress?
) where T : _ObjectiveCBridgeable, T._ObjectiveCType : NSItemProviderWriting
```

## See Also

### Registering objects

func registerObject(any NSItemProviderWriting, visibility: NSItemProviderRepresentationVisibility)

Adds representations of a specified object to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func registerObject(ofClass: any NSItemProviderWriting.Type, visibility: NSItemProviderRepresentationVisibility, loadHandler: (((any NSItemProviderWriting)?, (any Error)?) -> Void) -> Progress?)

Lazily adds representations of a specified object class to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func register&lt;T>(@autoclosure () -> T)

Adds representations of a specified transferable type to an item provider.

