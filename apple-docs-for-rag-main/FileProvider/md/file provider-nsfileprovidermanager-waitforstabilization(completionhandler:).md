

- File Provider
- NSFileProviderManager
-  waitForStabilization(completionHandler:) 

Instance Method

# waitForStabilization(completionHandler:)

Requests a notification after the domain stabilizes.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func waitForStabilization(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func waitForStabilization() async throws
```

## Parameters 

`completionHandler`  

A block that the system calls after pending changes to both the file system and the provider have completed. The system passes the following parameters:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func waitForStabilization() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to enforce a consistent state for testing. The system calls the completion handler after all the pending changes to the local cache and the remote storage have completed. The system waits on any changes that requested before the call to waitForStabilization(completionHandler:), but which haven’t completed yet.

Warning

Only use waitForStabilization(completionHandler:) for testing and debugging. Don’t call this method in a production app, due to its high performance cost.

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

func disconnect(reason: String, options: NSFileProviderManager.DisconnectionOptions, completionHandler: ((any Error)?) -> Void)

Disconnects the domain from the extension.

struct DisconnectionOptions

Options for disconnecting a domain from the extension.

func reconnect(completionHandler: ((any Error)?) -> Void)

Reconnects the domain with the extension.

func temporaryDirectoryURL() throws -> URL

Returns the URL of a directory that the File Provider extension can use to temporarily store files before passing them to the system.

