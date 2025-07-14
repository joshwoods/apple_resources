

- Foundation
- URLCredentialStorage
-  defaultCredential(for:) 

Instance Method

# defaultCredential(for:)

Returns the default credential for the specified protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func defaultCredential(for space: URLProtectionSpace) -> URLCredential?
```

## Parameters 

`space`  

The URL protection space of interest.

## Return Value

The default credential for `space` or `nil` if no default has been set.

## Discussion

If you override this method, also override getDefaultCredential(for:task:completionHandler:).

## See Also

### Getting and setting default credentials

func getDefaultCredential(for: URLProtectionSpace, task: URLSessionTask, completionHandler: (URLCredential?) -> Void)

Gets the default credential for the specified protection space, which is being accessed by the given task, and passes it to the provided completion handler.

func setDefaultCredential(URLCredential, for: URLProtectionSpace)

Sets the default credential for a specified protection space.

func setDefaultCredential(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Sets the default credential for a given protection space, which is being accessed by the given task.

