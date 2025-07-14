

- CallKit
- CXCallDirectoryManager
-  getEnabledStatusForExtension(withIdentifier:completionHandler:) 

Instance Method

# getEnabledStatusForExtension(withIdentifier:completionHandler:)

Asynchronously returns the enabled status of the extension with the specified identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func getEnabledStatusForExtension(
    withIdentifier identifier: String,
    completionHandler completion: @escaping (CXCallDirectoryManager.EnabledStatus, (any Error)?) -> Void
)
```

``` source
func enabledStatusForExtension(withIdentifier identifier: String) async throws -> CXCallDirectoryManager.EnabledStatus
```

## Parameters 

`identifier`  

The identifier for the call extension.

`completion`  

A block to be executed when the manager is finished determining the enabled status of the specified extension.

enabledStatus  
The enabled status of the extension. For possible values, see CXCallDirectoryManager.EnabledStatus.

error  
If an error occurred, an error object indicating how the check failed, otherwise `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func enabledStatusForExtension(withIdentifier identifier: String) async throws -> CXCallDirectoryManager.EnabledStatus
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with a Call Directory App Extension

func reloadExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Asynchronously reloads the extension with the specified identifier.

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

