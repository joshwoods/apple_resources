

- File Provider
- NSFileProviderManager
-  import(\_:fromDirectoryAt:completionHandler:) 

Type Method

# import(\_:fromDirectoryAt:completionHandler:)

Creates a new domain that takes ownership of on-disk data that your app previously managed without a file provider.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
class func `import`(
    _ domain: NSFileProviderDomain,
    fromDirectoryAt url: URL,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
class func `import`(
    _ domain: NSFileProviderDomain,
    fromDirectoryAt url: URL
) async throws
```

## Parameters 

`domain`  

The domain to import.

`url`  

A URL that points to the directory to import.

`completionHandler`  

A block that the system calls as soon as it creates the new domain. It takes the following parameters:

`error`  
If an error occurs, this object contains information about the error; otherwise, it’s `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func `import`(_ domain: NSFileProviderDomain, fromDirectoryAt url: URL) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to migrate an existing file hierarchy on disk to a NSFileProviderExtension without redownloading the data. After you call the method, the provided URL is no longer valid. The system has moved and now manages all of its contents.

If a domain with the same name already exists, the method fails with an NSFileWriteFileExistsError error. The URL remains untouched. If the system doesn’t allow the extension to request a migration, the method fails with an NSFeatureUnsupportedError error.

The system starts by moving the provided directory into its local cache, and then calls the completion handler. Then, for each item in the directory, it calls your extension’s createItem(basedOn:fields:contents:options:request:completionHandler:) with the mayAlreadyExist option.

When the import finishes, the system calls your extension’s importDidFinish(completionHandler:) method. If you call reimportItems(below:completionHandler:) before the import finishes, the system makes a single call to importDidFinish(completionHandler:) for both imports.

## See Also

### Working with domains

convenience init?(for: NSFileProviderDomain)

Returns a newly created file provider manager for the specified domain.

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

