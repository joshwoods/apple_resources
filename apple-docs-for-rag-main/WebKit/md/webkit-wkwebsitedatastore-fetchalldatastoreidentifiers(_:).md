

- WebKit
- WKWebsiteDataStore
-  fetchAllDataStoreIdentifiers(\_:) 

Type Method

# fetchAllDataStoreIdentifiers(\_:)

Fetches an array of identifiers from existing data stores that have identifiers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor
class func fetchAllDataStoreIdentifiers(_ completionHandler: @escaping @MainActor ([UUID]) -> Void)
```

``` source
@MainActor
class var allDataStoreIdentifiers: [UUID] { get async }
```

## Parameters 

`completionHandler`  

A block to invoke with the fetched list of unique identifiers.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class var allDataStoreIdentifiers: [UUID] { get async }
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

