

- Foundation
- NSItemProvider
-  registerDataRepresentation(forTypeIdentifier:visibility:loadHandler:) 

Instance Method

# registerDataRepresentation(forTypeIdentifier:visibility:loadHandler:)

Registers a data-backed representation for an item, specifiying item visibility and a load handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func registerDataRepresentation(
    forTypeIdentifier typeIdentifier: String,
    visibility: NSItemProviderRepresentationVisibility,
    loadHandler: @escaping (@escaping (Data?, (any Error)?) -> Void) -> Progress?
)
```

## See Also

### Registering data

func registerDataRepresentation(for: UTType, visibility: NSItemProviderRepresentationVisibility, loadHandler: ((Data?, (any Error)?) -> Void) -> Progress?)

Registers a data-backed representation for an item, specifiying item visibility and a load handler.

func registerItem(forTypeIdentifier: String, loadHandler: NSItemProvider.LoadHandler)

Lazily registers an item, according to the item provider type coercion policy.

