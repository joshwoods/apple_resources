

- Foundation
- URLCredentialStorage
-  credentials(for:) 

Instance Method

# credentials(for:)

Returns a dictionary containing the credentials for the specified protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func credentials(for space: URLProtectionSpace) -> [String : URLCredential]?
```

## Parameters 

`space`  

The protection space whose credentials you want to retrieve.

## Return Value

A dictionary containing the credentials for the specified protection space. The dictionary’s keys are user name strings, and each value is the corresponding URLCredential.

## Discussion

If you override this method, also override getCredentials(for:task:completionHandler:).

## See Also

### Retrieving credentials

var allCredentials: [URLProtectionSpace : [String : URLCredential]]

The credentials for all available protection spaces.

func getCredentials(for: URLProtectionSpace, task: URLSessionTask, completionHandler: ([String : URLCredential]?) -> Void)

Gets a dictionary containing the credentials for the specified protection space, on behalf of the given task, and passes the dictionary to the provided completion handler.

