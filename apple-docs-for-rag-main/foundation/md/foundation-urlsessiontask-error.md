

- Foundation
- URLSessionTask
-  error 

Instance Property

# error

An error object that indicates why the task failed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var error: (any Error)? { get }
```

## Discussion

This value is `nil` if the task is still active or if the transfer completed successfully.

## See Also

### Obtaining general task information

var currentRequest: URLRequest?

The URL request object currently being handled by the task.

var originalRequest: URLRequest?

The original request object passed when the task was created.

var response: URLResponse?

The server’s response to the currently active request.

var taskDescription: String?

An app-provided string value for the current task.

var taskIdentifier: Int

An identifier uniquely identifying the task within a given session.

