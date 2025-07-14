

- Foundation
- URLCredentialStorage
-  getDefaultCredential(for:task:completionHandler:) 

Instance Method

# getDefaultCredential(for:task:completionHandler:)

Gets the default credential for the specified protection space, which is being accessed by the given task, and passes it to the provided completion handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getDefaultCredential(
    for space: URLProtectionSpace,
    task: URLSessionTask,
    completionHandler: @escaping (URLCredential?) -> Void
)
```

``` source
func defaultCredential(
    for space: URLProtectionSpace,
    task: URLSessionTask
) async -> URLCredential?
```

## Parameters 

`space`  

The protection space of interest.

`task`  

The task seeking to use the protection space

`completionHandler`  

A completion handler that receives the default credential as its argument, or `nil` if there is no default credential for this combination of protection space and task.

## See Also

### Getting and setting default credentials

func defaultCredential(for: URLProtectionSpace) -> URLCredential?

Returns the default credential for the specified protection space.

func setDefaultCredential(URLCredential, for: URLProtectionSpace)

Sets the default credential for a specified protection space.

func setDefaultCredential(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Sets the default credential for a given protection space, which is being accessed by the given task.

