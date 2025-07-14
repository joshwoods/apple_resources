

- File Provider
- NSFileProviderManager
-  getUserVisibleURL(for:completionHandler:) 

Instance Method

# getUserVisibleURL(for:completionHandler:)

Returns the user-visible URL for an item.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func getUserVisibleURL(
    for itemIdentifier: NSFileProviderItemIdentifier,
    completionHandler: @escaping (URL?, (any Error)?) -> Void
)
```

``` source
func getUserVisibleURL(for itemIdentifier: NSFileProviderItemIdentifier) async throws -> URL
```

## Parameters 

`itemIdentifier`  

The item’s identifier.

`completionHandler`  

A block that the system calls after determining the item’s URL. The system passes the following parameters:

`userVisibleFile`  
The URL of the user visible file, or `nil` if an error occurs.

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func getUserVisibleURL(for itemIdentifier: NSFileProviderItemIdentifier) async throws -> URL
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Calling this method marks the process so that accessing the URL won’t materialize the item. Instead, any attempt to read or write to an unmaterialized item fails with a EDEADLK POSIX error.

## See Also

### Translating user-visible URLs

class func getIdentifierForUserVisibleFile(at: URL, completionHandler: (NSFileProviderItemIdentifier?, NSFileProviderDomainIdentifier?, (any Error)?) -> Void)

Returns the identifier and domain for a user-visible URL.

