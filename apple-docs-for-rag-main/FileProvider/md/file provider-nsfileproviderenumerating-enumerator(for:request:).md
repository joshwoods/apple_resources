

- File Provider
- NSFileProviderEnumerating
-  enumerator(for:request:) 

Instance Method

# enumerator(for:request:)

Tells the file provider to return an enumerator for the provided directory.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func enumerator(
    for containerItemIdentifier: NSFileProviderItemIdentifier,
    request: NSFileProviderRequest
) throws -> any NSFileProviderEnumerator
```

**Required**

## Parameters 

`containerItemIdentifier`  

The item identifier for the directory.

`request`  

An object that identifies the context of that request, such as the requesting app.

## Return Value

An enumerator for the specified directory.

## Mentioned in 

Synchronizing the File Provider Extension

## Discussion

The system calls this method to request an enumerator for the specified item.

Possible item identifiers include:

rootContainer  
The system passes this identifier when the user begins browsing your file provider’s content.

A directory’s itemIdentifier  
The system requests a new enumerator each time the user opens a new directory.

workingSet  
The system can request an enumerator so that it can sync the working set in the background.

A document’s itemIdentifier  
The system subscribes to live updates by requesting an enumerator for a document.

The trashContainer directory.  
The system passes this identifier when the user browses the contents of the trash. If your File Provider extension doesn’t support moving items to the trash, your implementation should throw or return an error.

Your implementation should create and return an NSFileProviderEnumerator object that provides the requested content.

### Handle Errors

If you can’t return the requested enumerator, you must throw an error in Swift, or if you return nil in Objective-C, you must set the `error` out parameter.

If the `containerItemIdentifier` parameter is trashContainer and your extension doesn’t support trashing items, then it should fail with the NSFeatureUnsupportedError error code from the NSCocoaErrorDomain domain. Additionally, make sure the items managed by your File Provider extension don’t have the allowsTrashing capability enabled.

If the `containerItemIdentifier` parameter doesn’t exist in your remote storage, you should fail with an NSFileProviderError.Code.noSuchItem error. The system then attempts to delete the item from disk.

If you pass NSFileProviderError.Code.notAuthenticated or NSFileProviderError.Code.serverUnreachable to the handler, the system presents an appropriate alert to the user, but doesn’t try to access the metadata until triggered again by the user.

The system considers any other errors to be transient, and automatically retries the method call.

