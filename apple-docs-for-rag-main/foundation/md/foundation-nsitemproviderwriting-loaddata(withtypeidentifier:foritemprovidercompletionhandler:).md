

- Foundation
- NSItemProviderWriting
-  loadData(withTypeIdentifier:forItemProviderCompletionHandler:) 

Instance Method

# loadData(withTypeIdentifier:forItemProviderCompletionHandler:)

Loads data of a particular type, identified by the given UTI.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func loadData(
    withTypeIdentifier typeIdentifier: String,
    forItemProviderCompletionHandler completionHandler: @escaping (Data?, (any Error)?) -> Void
) -> Progress?
```

**Required**

## Parameters 

`typeIdentifier`  

The uniform type identifier (UTI) identifying the type of data to load.

`completionHandler`  

The handler that’s called after the data is loaded.

## Return Value

The progress of the data load process.

## Discussion

When the system calls this method, the `typeIdentifier` parameter is set to one of the elements in the `writableTypeIdentifiersForItemProvider` array.

