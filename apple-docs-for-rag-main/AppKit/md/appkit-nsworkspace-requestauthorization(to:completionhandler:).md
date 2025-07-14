

- AppKit
- NSWorkspace
-  requestAuthorization(to:completionHandler:) 

Instance Method

# requestAuthorization(to:completionHandler:)

Requests authorization to perform a privileged file operation.

macOS 10.14+

``` source
func requestAuthorization(
    to type: NSWorkspace.AuthorizationType,
    completionHandler: @escaping (NSWorkspace.Authorization?, (any Error)?) -> Void
)
```

``` source
func requestAuthorization(to type: NSWorkspace.AuthorizationType) async throws -> NSWorkspace.Authorization
```

## Parameters 

`type`  

The type of file operation to perform.

`completionHandler`  

The completion handler to call when the authorization request is completed.

The completion handler takes two parameters:

authorization  
The authorization granted for this app. Use it when creating a new FileManager with init(authorization:).

error  
`nil` if the app is authorized; otherwise, a pointer to the authorization error.

## Discussion

## See Also

### Performing Privileged Operations

class Authorization

The authorization granted to the app by the user.

enum AuthorizationType

The types of privileged file operations that can be authorized by the user.

