

- Foundation
- NSItemProvider
-  register(\_:) 

Instance Method

# register(\_:)

Adds representations of a specified transferable type to an item provider.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func register(_ transferable: @autoclosure @escaping () -> T) where T : Transferable
```

## See Also

### Registering objects

func registerObject(any NSItemProviderWriting, visibility: NSItemProviderRepresentationVisibility)

Adds representations of a specified object to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func registerObject(ofClass: any NSItemProviderWriting.Type, visibility: NSItemProviderRepresentationVisibility, loadHandler: (((any NSItemProviderWriting)?, (any Error)?) -> Void) -> Progress?)

Lazily adds representations of a specified object class to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func registerObject&lt;T>(ofClass: T.Type, visibility: NSItemProviderRepresentationVisibility, loadHandler: ((T?, (any Error)?) -> Void) -> Progress?)

Lazily adds representations of a specified object type to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

