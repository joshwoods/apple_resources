

- WebKit
- WKWebsiteDataStore
-  remove(forIdentifier:completionHandler:) 

Type Method

# remove(forIdentifier:completionHandler:)

Removes the data store that matches the identifier you provide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
class func remove(
    forIdentifier identifier: UUID,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
@MainActor
class func remove(forIdentifier identifier: UUID) async throws
```

## Parameters 

`identifier`  

An identifier that uniquely identifies a data store.

`completionHandler`  

A block the system invokes after it removes the data store. This block has no return value, and takes the following parameter:

error  
An error, if the system could not remove the data store.

## Discussion

Call this method to remove the data store for the unique identifier. Release any WKWebView instances using the data store before you call this method. If the system cannot complete removal of the data store, this throws an error.

