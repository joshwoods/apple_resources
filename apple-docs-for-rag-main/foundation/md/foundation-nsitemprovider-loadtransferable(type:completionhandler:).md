

- Foundation
- NSItemProvider
-  loadTransferable(type:completionHandler:) 

Instance Method

# loadTransferable(type:completionHandler:)

Asynchronously loads an object of a specified transferable type to an item provider, returning a progress object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func loadTransferable(
    type transferableType: T.Type,
    completionHandler: @escaping (Result) -> Void
) -> Progress where T : Transferable
```

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

func loadInPlaceFileRepresentation(forTypeIdentifier: String, completionHandler: (URL?, Bool, (any Error)?) -> Void) -> Progress

Asynchronously opens a file in place, if possible, returning a progress object.

func loadObject(ofClass: any NSItemProviderReading.Type, completionHandler: ((any NSItemProviderReading)?, (any Error)?) -> Void) -> Progress

Asynchronously loads an object of a specified class to an item provider, returning a progress object.

func loadObject&lt;T>(ofClass: T.Type, completionHandler: (T?, (any Error)?) -> Void) -> Progress

Asynchronously loads an object of a specified class to an item provider, returning a progress object.

