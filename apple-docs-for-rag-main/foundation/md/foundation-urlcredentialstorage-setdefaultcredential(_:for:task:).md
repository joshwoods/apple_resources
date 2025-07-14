

- Foundation
- URLCredentialStorage
-  setDefaultCredential(\_:for:task:) 

Instance Method

# setDefaultCredential(\_:for:task:)

Sets the default credential for a given protection space, which is being accessed by the given task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setDefaultCredential(
    _ credential: URLCredential,
    for protectionSpace: URLProtectionSpace,
    task: URLSessionTask
)
```

## Parameters 

`credential`  

The URL credential to set as the default for the protection space. If the receiver does not contain `credential` in the specified protection space it will be added.

`protectionSpace`  

The protection space whose default credential is being set.

`task`  

The task accessing the specified protection space. Subclasses of URLCredentialStorage may use the request URL or other properties of this task to affect how the default credential is stored.

## See Also

### Getting and setting default credentials

func defaultCredential(for: URLProtectionSpace) -> URLCredential?

Returns the default credential for the specified protection space.

func getDefaultCredential(for: URLProtectionSpace, task: URLSessionTask, completionHandler: (URLCredential?) -> Void)

Gets the default credential for the specified protection space, which is being accessed by the given task, and passes it to the provided completion handler.

func setDefaultCredential(URLCredential, for: URLProtectionSpace)

Sets the default credential for a specified protection space.

