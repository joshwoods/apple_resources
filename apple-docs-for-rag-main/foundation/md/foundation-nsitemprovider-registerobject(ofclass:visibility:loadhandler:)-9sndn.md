

- Foundation
- NSItemProvider
-  registerObject(ofClass:visibility:loadHandler:) 

Instance Method

# registerObject(ofClass:visibility:loadHandler:)

Lazily adds representations of a specified object class to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func registerObject(
    ofClass aClass: any NSItemProviderWriting.Type,
    visibility: NSItemProviderRepresentationVisibility,
    loadHandler: @escaping (@escaping ((any NSItemProviderWriting)?, (any Error)?) -> Void) -> Progress?
)
```

## See Also

### Registering objects

func registerObject(any NSItemProviderWriting, visibility: NSItemProviderRepresentationVisibility)

Adds representations of a specified object to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func registerObject&lt;T>(ofClass: T.Type, visibility: NSItemProviderRepresentationVisibility, loadHandler: ((T?, (any Error)?) -> Void) -> Progress?)

Lazily adds representations of a specified object type to an item provider, based on the object’s implementation of the item provider writing protocol, and adhering to a visibility specification.

func register&lt;T>(@autoclosure () -> T)

Adds representations of a specified transferable type to an item provider.

