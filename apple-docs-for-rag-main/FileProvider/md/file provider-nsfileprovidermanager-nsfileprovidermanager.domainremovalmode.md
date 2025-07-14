

- File Provider
- NSFileProviderManager
-  NSFileProviderManager.DomainRemovalMode 

Enumeration

# NSFileProviderManager.DomainRemovalMode

A mode indicating how the system handles user data when removing a domain.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
enum DomainRemovalMode
```

## Topics

### Options

case removeAll

Deletes all items in the domain.

case preserveDirtyUserData

Deletes the domain but keeps any items with unsynced, local changes.

case preserveDownloadedUserData

Deletes the domain, but keeps the downloaded user data.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

