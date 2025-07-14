

- File Provider
- NSFileProviderManager
-  disconnect(reason:options:completionHandler:) 

Instance Method

# disconnect(reason:options:completionHandler:)

Disconnects the domain from the extension.

macOS 11.0+

``` source
func disconnect(
    reason localizedReason: String,
    options: NSFileProviderManager.DisconnectionOptions = [],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func disconnect(
    reason localizedReason: String,
    options: NSFileProviderManager.DisconnectionOptions = []
) async throws
```

## Parameters 

`localizedReason`  

A localized string that describes the reason for disconnecting the domain.

`options`  

Options for the disconnection. For a complete list of valid options, see NSFileProviderManager.DisconnectionOptions.

`completionHandler`  

A block that the system calls after disconnecting the domain. The block takes the following parameter:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func disconnect(reason localizedReason: String, options: NSFileProviderManager.DisconnectionOptions = []) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method to disconnect the domain from the extension. While the domain is disconnected, the user can continue to browse its content, but the extension no longer receives updates about changes.

Call the reconnect(completionHandler:) method to reconnect the domain.

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

class func remove(NSFileProviderDomain, mode: NSFileProviderManager.DomainRemovalMode, completionHandler: (URL?, (any Error)?) -> Void)

Removes a domain from the File Provider extension using the specified options.

class func removeAllDomains(completionHandler: ((any Error)?) -> Void)

Removes all domains from the File Provider extension.

enum DomainRemovalMode

A mode indicating how the system handles user data when removing a domain.

struct DisconnectionOptions

Options for disconnecting a domain from the extension.

func reconnect(completionHandler: ((any Error)?) -> Void)

Reconnects the domain with the extension.

func waitForStabilization(completionHandler: ((any Error)?) -> Void)

Requests a notification after the domain stabilizes.

func temporaryDirectoryURL() throws -> URL

Returns the URL of a directory that the File Provider extension can use to temporarily store files before passing them to the system.

