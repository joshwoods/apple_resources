

- File Provider
- NSFileProviderManager
-  placeholderURL(for:) 

Type Method

# placeholderURL(for:)

Returns a placeholder URL for a given document URL.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
class func placeholderURL(for url: URL) -> URL
```

## Parameters 

`url`  

The document URL to be converted.

## Return Value

A placeholder URL for the given document.

## Discussion

This method maps file URLs into their corresponding placeholder URLs. You typically call this method to generate the placeholder URL before calling writePlaceholder(at:withMetadata:).

Note

While this method is available on macOS 11+, you don’t need to use it when creating a file provider extension that adopts the NSFileProviderReplicatedExtension protocol.

## See Also

### Performing actions

class func writePlaceholder(at: URL, withMetadata: NSFileProviderItem) throws

Writes a document placeholder with the provided metadata.

func register(URLSessionTask, forItemWithIdentifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Registers the URL session task responsible for the specified item.

func signalEnumerator(for: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Alerts the system to changes in the specified folder’s content.

func waitForChanges(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Requests a notification after the system completes all the specified changes.

func globalProgress(for: Progress.FileOperationKind) -> Progress

Returns a progress object that tracks either the uploading or downloading of items from the File Provider extension’s remote storage.

