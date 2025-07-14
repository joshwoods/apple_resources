

- File Provider
-  NSFileProviderManager 

Class

# NSFileProviderManager

A manager object that you use to communicate with the file provider from either your app or your File Provider extension.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
class NSFileProviderManager
```

## Mentioned in 

Signaling Changes for User-Driven Actions

Synchronizing the File Provider Extension

## Topics

### Accessing File Provider data

class var `default`: NSFileProviderManager

A property that returns the shared file provider manager object.

var documentStorageURL: URL

The root URL for all shared documents.

var providerIdentifier: String

A purpose identifier for coordinated reads and writes.

### Translating user-visible URLs

func getUserVisibleURL(for: NSFileProviderItemIdentifier, completionHandler: (URL?, (any Error)?) -> Void)

Returns the user-visible URL for an item.

class func getIdentifierForUserVisibleFile(at: URL, completionHandler: (NSFileProviderItemIdentifier?, NSFileProviderDomainIdentifier?, (any Error)?) -> Void)

Returns the identifier and domain for a user-visible URL.

### Working with items

func reimportItems(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Tells the system to reimport the item and its content recursively.

func evictItem(identifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Asks the system to remove an item from its cache.

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?) async throws

func requestDownloadForItem(withIdentifier: NSFileProviderItemIdentifier, requestedRange: NSRange?, completionHandler: ((any Error)?) -> Void)

func requestModification(of: NSFileProviderItemFields, forItemWithIdentifier: NSFileProviderItemIdentifier, options: NSFileProviderModifyItemOptions, completionHandler: ((any Error)?) -> Void)

func enumeratorForMaterializedItems() -> any NSFileProviderEnumerator

Returns an enumerator for all the items the system currently stores on disk.

func enumeratorForPendingItems() -> any NSFileProviderPendingSetEnumerator

Returns an enumerator for the set of pending items.

### Performing actions

class func placeholderURL(for: URL) -> URL

Returns a placeholder URL for a given document URL.

class func writePlaceholder(at: URL, withMetadata: NSFileProviderItem) throws

Writes a document placeholder with the provided metadata.

func register(URLSessionTask, forItemWithIdentifier: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Registers the URL session task responsible for the specified item.

func signalEnumerator(for: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Alerts the system to changes in the specified folder’s content.

func waitForChanges(below: NSFileProviderItemIdentifier, completionHandler: ((any Error)?) -> Void)

Requests a notification after the system completes all the specified changes.

func globalProgress(for: Progress.FileOperationKind) -> Progress

Returns a progress object that tracks either the uploading or downloading of items from the File Provider extension’s remote storage.

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

func temporaryDirectoryURL() throws -> URL

Returns the URL of a directory that the File Provider extension can use to temporarily store files before passing them to the system.

### Syncing Desktop and Documents folders

func claimKnownFolders(NSFileProviderKnownFolderLocations, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the domain to sync the specified known folders.

func releaseKnownFolders(NSFileProviderKnownFolders, localizedReason: String, completionHandler: ((any Error)?) -> Void)

Asks the system to stop replicating the specified known folders in the domain.

struct NSFileProviderKnownFolders

Constants that identify known folders.

class NSFileProviderKnownFolderLocations

A class for working with known-folder locations.

protocol NSFileProviderKnownFolderSupporting

A protocol that defines the interface for sharing known-folder locations with the system.

### Working with external volumes

func stateDirectoryURL() throws -> URL

Returns a URL for a directory for storing state information for the domain.

class func checkDomainsCanBeStoredOnVolume(at: URL) throws -> NSFileProviderManager.EligibilityResult

Checks whether the specified URL is eligible for storing a domain.

enum EligibilityResult

Constants that specify whether a URL is eligible for storing a domain.

protocol NSFileProviderExternalVolumeHandling

A protocol that defines the interface for handling external volumes.

### Using services

func getService(named: NSFileProviderServiceName, for: NSFileProviderItemIdentifier, completionHandler: (NSFileProviderService?, (any Error)?) -> Void)

### Testing

func listAvailableTestingOperations() throws -> [any NSFileProviderTestingOperation]

Lists all the operations that are ready for scheduling.

func run([any NSFileProviderTestingOperation]) throws -> [AnyHashable : any Error]

Asks the system to schedule and execute the specified operations.

### Handling errors

func signalErrorResolved(any Error, completionHandler: ((any Error)?) -> Void)

Indicates a resolved error.

### Collecting diagnostic reports

func requestDiagnosticCollection(for: NSFileProviderItemIdentifier, errorReason: any Error, completionHandler: ((any Error)?) -> Void)

Requests a diagnostics collection for use when working directly with Apple to improve sync behavior.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

