

- Foundation
- URLCredentialStorage
-  setDefaultCredential(\_:for:) 

Instance Method

# setDefaultCredential(\_:for:)

Sets the default credential for a specified protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setDefaultCredential(
    _ credential: URLCredential,
    for space: URLProtectionSpace
)
```

## Parameters 

`credential`  

The URL credential to set as the default for `space`. If the receiver does not contain `credential` in the specified protection space it will be added.

`space`  

The protection space whose default credential is being set.

## Discussion

If you override this method, also override setDefaultCredential(_:for:task:).

## See Also

### Getting and setting default credentials

func defaultCredential(for: URLProtectionSpace) -> URLCredential?

Returns the default credential for the specified protection space.

func getDefaultCredential(for: URLProtectionSpace, task: URLSessionTask, completionHandler: (URLCredential?) -> Void)

Gets the default credential for the specified protection space, which is being accessed by the given task, and passes it to the provided completion handler.

func setDefaultCredential(URLCredential, for: URLProtectionSpace, task: URLSessionTask)

Sets the default credential for a given protection space, which is being accessed by the given task.

