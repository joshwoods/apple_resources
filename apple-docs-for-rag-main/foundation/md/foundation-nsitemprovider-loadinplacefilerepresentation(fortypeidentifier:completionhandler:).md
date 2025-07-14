

- Foundation
- NSItemProvider
-  loadInPlaceFileRepresentation(forTypeIdentifier:completionHandler:) 

Instance Method

# loadInPlaceFileRepresentation(forTypeIdentifier:completionHandler:)

Asynchronously opens a file in place, if possible, returning a progress object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func loadInPlaceFileRepresentation(
    forTypeIdentifier typeIdentifier: String,
    completionHandler: @escaping (URL?, Bool, (any Error)?) -> Void
) -> Progress
```

## Discussion

The system sets the `isInPlace` parameter to true if the system successfully opened the file in place, or false if it made a local copy. In either case, you must access the returned URL using an NSFileCoordinator object.

If the system created a local copy of a file, it will be automatically deleted after your file coordinator relinquishes its read access to the file.

## See Also

### Loading the provider’s contents

func loadItem(forTypeIdentifier: String, options: [AnyHashable : Any]?, completionHandler: NSItemProvider.CompletionHandler?)

Loads the item’s data and coerces it to the specified type.

func loadDataRepresentation(forTypeIdentifier: String, completionHandler: (Data?, (any Error)?) -> Void) -> Progress

Asynchronously copies the provided, typed data into a generic data object, returning a progress object.

func loadDataRepresentation(for: UTType, completionHandler: (Data?, (any Error)?) -> Void) -> Progress

Asynchronously copies the universal type data into a generic data object, returning a progress object.

func loadFileRepresentation(forTypeIdentifier: String, completionHandler: (URL?, (any Error)?) -> Void) -> Progress

Asynchronously writes a copy of the provided, typed data to a temporary file, returning a progress object.

func loadFileRepresentation(for: UTType, openInPlace: Bool, completionHandler: (URL?, Bool, (any Error)?) -> Void) -> Progress

Asynchronously writes a copy of the universal type data to a temporary file, returning a progress object.

func loadObject(ofClass: any NSItemProviderReading.Type, completionHandler: ((any NSItemProviderReading)?, (any Error)?) -> Void) -> Progress

Asynchronously loads an object of a specified class to an item provider, returning a progress object.

func loadObject&lt;T>(ofClass: T.Type, completionHandler: (T?, (any Error)?) -> Void) -> Progress

Asynchronously loads an object of a specified class to an item provider, returning a progress object.

func loadTransferable&lt;T>(type: T.Type, completionHandler: (Result&lt;T, any Error>) -> Void) -> Progress

Asynchronously loads an object of a specified transferable type to an item provider, returning a progress object.

