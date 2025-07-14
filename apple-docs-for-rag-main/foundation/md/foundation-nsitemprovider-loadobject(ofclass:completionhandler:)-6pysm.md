

- Foundation
- NSItemProvider
-  loadObject(ofClass:completionHandler:) 

Instance Method

# loadObject(ofClass:completionHandler:)

Asynchronously loads an object of a specified class to an item provider, returning a progress object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
@preconcurrency
func loadObject(
    ofClass: T.Type,
    completionHandler: @escaping (T?, (any Error)?) -> Void
) -> Progress where T : _ObjectiveCBridgeable, T._ObjectiveCType : NSItemProviderReading
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

func loadTransferable&lt;T>(type: T.Type, completionHandler: (Result&lt;T, any Error>) -> Void) -> Progress

Asynchronously loads an object of a specified transferable type to an item provider, returning a progress object.

