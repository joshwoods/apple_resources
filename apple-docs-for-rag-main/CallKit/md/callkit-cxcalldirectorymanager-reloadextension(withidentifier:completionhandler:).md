

- CallKit
- CXCallDirectoryManager
-  reloadExtension(withIdentifier:completionHandler:) 

Instance Method

# reloadExtension(withIdentifier:completionHandler:)

Asynchronously reloads the extension with the specified identifier.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func reloadExtension(
    withIdentifier identifier: String,
    completionHandler completion: (((any Error)?) -> Void)? = nil
)
```

``` source
func reloadExtension(withIdentifier identifier: String) async throws
```

## Parameters 

`identifier`  

The identifier for the call extension.

`completion`  

A block to be executed when the manager is finished reloading the specified extension.

error  
If an error occurred, an error object indicating how reloading failed, otherwise `nil`.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func reloadExtension(withIdentifier identifier: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Working with a Call Directory App Extension

func getEnabledStatusForExtension(withIdentifier: String, completionHandler: (CXCallDirectoryManager.EnabledStatus, (any Error)?) -> Void)

Asynchronously returns the enabled status of the extension with the specified identifier.

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

