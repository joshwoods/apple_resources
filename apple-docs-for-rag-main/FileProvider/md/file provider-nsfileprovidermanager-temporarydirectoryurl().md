

- File Provider
- NSFileProviderManager
-  temporaryDirectoryURL() 

Instance Method

# temporaryDirectoryURL()

Returns the URL of a directory that the File Provider extension can use to temporarily store files before passing them to the system.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
func temporaryDirectoryURL() throws -> URL
```

## Discussion

The system guarantees that the temporary URL refers to a directory on the same volume as the user-visible URL so that the system can automatically clone or move files between the temporary URL and the user-visible URL. For example, the File Provider extension can use the temporary directory to store content passed to the createItem(basedOn:fields:contents:options:request:completionHandler:) or modifyItem(_:baseVersion:changedFields:contents:options:request:completionHandler:) methods.

When you implement your File Provider extension’s fetchContents(for:version:request:completionHandler:) method, the URL you pass to the completion handler must be on the same volume as the temporary directory, so the system can clone it to provide the content for the dataless item.

This method fails if the system can’t find a suitable directory, for example, if the domain doesn’t exist. However, it can’t fail if the file provider has an active instance for the specified domain.

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

func waitForStabilization(completionHandler: ((any Error)?) -> Void)

Requests a notification after the domain stabilizes.

