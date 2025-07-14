

- File Provider
- NSFileProviderManager
-  getIdentifierForUserVisibleFile(at:completionHandler:) 

Type Method

# getIdentifierForUserVisibleFile(at:completionHandler:)

Returns the identifier and domain for a user-visible URL.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
class func getIdentifierForUserVisibleFile(
    at url: URL,
    completionHandler: @escaping (NSFileProviderItemIdentifier?, NSFileProviderDomainIdentifier?, (any Error)?) -> Void
)
```

``` source
class func identifierForUserVisibleFile(at url: URL) async throws -> (NSFileProviderItemIdentifier, NSFileProviderDomainIdentifier)
```

## Parameters 

`url`  

The URL of the item.

`completionHandler`  

A block that the system calls after it gets the items identifier. It has the following parameters:

`itemIdentifier`  
The item’s identifier.

`domainIdentifier`  
The identifier for the item’s domain.

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func identifierForUserVisibleFile(at url: URL) async throws -> (NSFileProviderItemIdentifier, NSFileProviderDomainIdentifier)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If the URL doesn’t refer to an item managed by your File Provider extension, the system returns a NSFileNoSuchFileError error.

## See Also

### Translating user-visible URLs

func getUserVisibleURL(for: NSFileProviderItemIdentifier, completionHandler: (URL?, (any Error)?) -> Void)

Returns the user-visible URL for an item.

