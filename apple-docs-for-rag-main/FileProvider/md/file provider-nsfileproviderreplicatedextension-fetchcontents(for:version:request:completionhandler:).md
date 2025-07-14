

- File Provider
- NSFileProviderReplicatedExtension
-  fetchContents(for:version:request:completionHandler:) 

Instance Method

# fetchContents(for:version:request:completionHandler:)

Tells the file provider to download the requested item from remote storage.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func fetchContents(
    for itemIdentifier: NSFileProviderItemIdentifier,
    version requestedVersion: NSFileProviderItemVersion?,
    request: NSFileProviderRequest,
    completionHandler: @escaping (URL?, NSFileProviderItem?, (any Error)?) -> Void
) -> Progress
```

**Required**

## Parameters 

`itemIdentifier`  

The item to fetch.

`requestedVersion`  

The version of the item. If this is `nil`, download the latest version.

`request`  

An object that identifies the context of that request, such as the requesting app.

`completionHandler`  

A block that you call after downloading the item from your remote storage. You pass the following parameters:

`fileContents`  
A URL to the item’s contents.

`item`  
The downloaded item.

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Return Value

An item that tracks your extension’s progress. The system automatically calls cancel() on the progress object when an error occurs, or when the system or user cancels the download.

## Mentioned in 

Synchronizing the File Provider Extension

## Discussion

The system initially learns about available items through enumerations; however, the enumeration only provides the item’s metadata. When the user accesses the item, the system needs to download the full contents from your remote store. After you call the completion handler, the system takes complete control over the local copy.

Note

The URL you pass to the completion handler must be on the same volume as the URL returned by the file provider manager’s temporaryDirectoryURL() method, so that the system can clone it to provide the content for the dataless item.

If the `requestedVersion` parameter is not `nil`, you must return the specified version of the item, or return an error. If the parameter is `nil`, return a version that is the same or newer than the most recent version enumerated to the system. In either case, the contentVersion of the NSFileProviderItem passed to the completion handler must match the version you return.

If your extension doesn’t recognize the item, pass NSFileProviderError.Code.noSuchItem to the handler. The system assumes the item is no longer in the domain, and attempts to delete the local copy. If the delete attempt fails because the item has local changes, the system reimports the item by calling createItem(basedOn:fields:contents:options:request:completionHandler:).

If you pass NSFileProviderError.Code.notAuthenticated or NSFileProviderError.Code.serverUnreachable to the handler, the system presents an appropriate alert to the user, but doesn’t try to access the metadata until triggered again by the user.

If the user deletes the item before the download completes, the system calls the progress object’s cancel() method. Your file provider should stop fetching the item, and pass NSUserCancelledError to the handler.

The system considers any other errors to be transient, and automatically retries the method call.

## See Also

### Accessing Remote Content

func item(for: NSFileProviderItemIdentifier, request: NSFileProviderRequest, completionHandler: (NSFileProviderItem?, (any Error)?) -> Void) -> Progress

Asks the file provider for the metadata of the provided item.

**Required**

