

- Foundation
- URLCredentialStorage
-  allCredentials 

Instance Property

# allCredentials

The credentials for all available protection spaces.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allCredentials: [URLProtectionSpace : [String : URLCredential]] { get }
```

## Discussion

The dictionary has keys corresponding to the URLProtectionSpace instances. The values are dictionaries where the keys are user name strings, and each value is the corresponding URLCredential instances.

## See Also

### Retrieving credentials

func credentials(for: URLProtectionSpace) -> [String : URLCredential]?

Returns a dictionary containing the credentials for the specified protection space.

func getCredentials(for: URLProtectionSpace, task: URLSessionTask, completionHandler: ([String : URLCredential]?) -> Void)

Gets a dictionary containing the credentials for the specified protection space, on behalf of the given task, and passes the dictionary to the provided completion handler.

