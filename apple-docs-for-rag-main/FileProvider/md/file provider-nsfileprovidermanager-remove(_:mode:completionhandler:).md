

- File Provider
- NSFileProviderManager
-  remove(\_:mode:completionHandler:) 

Type Method

# remove(\_:mode:completionHandler:)

Removes a domain from the File Provider extension using the specified options.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
class func remove(
    _ domain: NSFileProviderDomain,
    mode: NSFileProviderManager.DomainRemovalMode,
    completionHandler: @escaping (URL?, (any Error)?) -> Void
)
```

``` source
class func remove(
    _ domain: NSFileProviderDomain,
    mode: NSFileProviderManager.DomainRemovalMode
) async throws -> URL?
```

## Parameters 

`domain`  

The domain to remove.

`mode`  

An option that determines how the system handles user data. For a complete list of options, see NSFileProviderManager.DomainRemovalMode.

`completionHandler`  

A block that the system calls after removing the domain. It takes the following parameter:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func remove(_ domain: NSFileProviderDomain, mode: NSFileProviderManager.DomainRemovalMode) async throws -> URL?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with domains

convenience init?(for: NSFileProviderDomain)

Returns a newly created file provider manager for the specified domain.

class func `import`(NSFileProviderDomain, fromDirectoryAt: URL, completionHandler: ((any Error)?) -> Void)

Creates a new domain that takes ownership of on-disk data that your app previously managed without a file provider.

class func add(NSFileProviderDomain, completionHandler: ((any Error)?) -> Void)

Adds a domain to the File Provider extension.

class func getDomainsWithCompletionHandler(([NSFileProviderDomain], (any Error)?) -> Void)

Returns all of the File Provider extension’s domains.

class func remove(NSFileProviderDomain, completionHandler: ((any Error)?) -> Void)

Removes a domain from the File Provider extension.

class func removeAllDomains(completionHandler: ((any Error)?) -> Void)

Removes all domains from the File Provider extension.

enum DomainRemovalMode

A mode indicating how the system handles user data when removing a domain.

func disconnect(reason: String, options: NSFileProviderManager.DisconnectionOptions, completionHandler: ((any Error)?) -> Void)

Disconnects the domain from the extension.

struct DisconnectionOptions

Options for disconnecting a domain from the extension.

func reconnect(completionHandler: ((any Error)?) -> Void)

Reconnects the domain with the extension.

func waitForStabilization(completionHandler: ((any Error)?) -> Void)

Requests a notification after the domain stabilizes.

func temporaryDirectoryURL() throws -> URL

Returns the URL of a directory that the File Provider extension can use to temporarily store files before passing them to the system.

