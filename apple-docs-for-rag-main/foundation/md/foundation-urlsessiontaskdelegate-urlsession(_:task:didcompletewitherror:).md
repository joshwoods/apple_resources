

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:didCompleteWithError:) 

Instance Method

# urlSession(\_:task:didCompleteWithError:)

Tells the delegate that the task finished transferring data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    didCompleteWithError error: (any Error)?
)
```

## Parameters 

`session`  

The session containing the task that has finished transferring data.

`task`  

The task that has finished transferring data.

`error`  

If an error occurred, an error object indicating how the transfer failed, otherwise `NULL`.

## Mentioned in 

Pausing and resuming downloads

Downloading files from websites

Pausing and resuming uploads

Fetching website data into memory

## Discussion

The only errors your delegate receives through the `error` parameter are client-side errors, such as being unable to resolve the hostname or connect to the host. To check for server-side errors, inspect the response property of the `task` parameter received by this callback.

