

- Foundation
- URLCredentialStorage
-  getCredentials(for:task:completionHandler:) 

Instance Method

# getCredentials(for:task:completionHandler:)

Gets a dictionary containing the credentials for the specified protection space, on behalf of the given task, and passes the dictionary to the provided completion handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getCredentials(
    for protectionSpace: URLProtectionSpace,
    task: URLSessionTask,
    completionHandler: @escaping ([String : URLCredential]?) -> Void
)
```

``` source
func credentials(
    for protectionSpace: URLProtectionSpace,
    task: URLSessionTask
) async -> [String : URLCredential]?
```

## Parameters 

`protectionSpace`  

The protection space whose credentials you want to retrieve.

`task`  

The task accessing the specified protection space.

`completionHandler`  

A completion handler that receives a single argument with the credentials for the specified protection space and task. The dictionary’s keys are user name strings, and the corresponding value is a URLCredential. If no credential has been set for this space, the argument to the completion handler is `nil`.

## See Also

### Retrieving credentials

var allCredentials: [URLProtectionSpace : [String : URLCredential]]

The credentials for all available protection spaces.

func credentials(for: URLProtectionSpace) -> [String : URLCredential]?

Returns a dictionary containing the credentials for the specified protection space.

