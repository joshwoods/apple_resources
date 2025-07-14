

- Swift
- DecodingError
-  dataCorruptedError(forKey:in:debugDescription:) 

Type Method

# dataCorruptedError(forKey:in:debugDescription:)

Returns a new `.dataCorrupted` error using a constructed coding path and the given debug description.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func dataCorruptedError(
    forKey key: C.Key,
    in container: C,
    debugDescription: String
) -> DecodingError where C : KeyedDecodingContainerProtocol
```

## Return Value

A new `.dataCorrupted` error with the given information.

## Discussion

The coding path for the returned error is constructed by appending the given key to the given container’s coding path.

- param key: The key which caused the failure.

- param container: The container in which the corrupted data was accessed.

- param debugDescription: A description of the error to aid in debugging.

