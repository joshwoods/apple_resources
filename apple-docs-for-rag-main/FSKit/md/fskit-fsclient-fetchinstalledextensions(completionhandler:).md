

- FSKit
- FSClient
-  fetchInstalledExtensions(completionHandler:) 

Instance Method

# fetchInstalledExtensions(completionHandler:)

Asynchronously retrieves an list of installed file system modules.

macOS 15.4+

``` source
func fetchInstalledExtensions(completionHandler: @escaping ([FSModuleIdentity]?, (any Error)?) -> Void)
```

``` source
var installedExtensions: [FSModuleIdentity] { get async throws }
```

## Parameters 

`completionHandler`  

A block or closure that executes when FSKit finishes its fetch process. If the fetch succeeds, the first parameter contains an array of FSModuleIdentity instances that identify installed modules. If the fetch fails, the second parameter contains an error detailing the failure.

## Discussion

In Swift, you can either call this method and pass a completion handler closure, or get the value of the `installedExtensions` property with the `async` keyword.

## See Also

### Discovering installed extensions

class FSModuleIdentity

An installed file system module.

