

- Foundation
- NSItemProvider
-  registerFileRepresentation(forTypeIdentifier:fileOptions:visibility:loadHandler:) 

Instance Method

# registerFileRepresentation(forTypeIdentifier:fileOptions:visibility:loadHandler:)

Registers a file-backed representation for an item, specifying file options, item visibility, and a load handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func registerFileRepresentation(
    forTypeIdentifier typeIdentifier: String,
    fileOptions: NSItemProviderFileOptions = [],
    visibility: NSItemProviderRepresentationVisibility,
    loadHandler: @escaping (@escaping (URL?, Bool, (any Error)?) -> Void) -> Progress?
)
```

## Discussion

If a destination app must access the represented file using a file coordinator, set the `coordinated` parameter in the load handler block to true.

To offer a representation backed by a file provider, return an NSURL object that points to your app’s file provider’s container. The file provider extension is then invoked to retrieve the file when requested.

To offer a representation backed by a file to open in place, set the fileOptions parameter to a value of openInPlace; in addition, return an NSURL object that points to your app’s file provider’s container. Open-in-place support requires that the file provider is visible in the Files app.

## See Also

### Registering files

func registerFileRepresentation(for: UTType, visibility: NSItemProviderRepresentationVisibility, openInPlace: Bool, loadHandler: ((URL?, Bool, (any Error)?) -> Void) -> Progress?)

Registers a file-backed representation for an item with item visibility, an open-in-place option, and a load handler.

