

- Foundation
- NSItemProvider
-  registerDataRepresentation(for:visibility:loadHandler:) 

Instance Method

# registerDataRepresentation(for:visibility:loadHandler:)

Registers a data-backed representation for an item, specifiying item visibility and a load handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func registerDataRepresentation(
    for contentType: UTType,
    visibility: NSItemProviderRepresentationVisibility = .all,
    loadHandler: @escaping (@escaping (Data?, (any Error)?) -> Void) -> Progress?
)
```

## See Also

### Registering data

func registerDataRepresentation(forTypeIdentifier: String, visibility: NSItemProviderRepresentationVisibility, loadHandler: ((Data?, (any Error)?) -> Void) -> Progress?)

Registers a data-backed representation for an item, specifiying item visibility and a load handler.

func registerItem(forTypeIdentifier: String, loadHandler: NSItemProvider.LoadHandler)

Lazily registers an item, according to the item provider type coercion policy.

