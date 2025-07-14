

- Foundation
- URLSessionTask
-  taskDescription 

Instance Property

# taskDescription

An app-provided string value for the current task.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var taskDescription: String? { get set }
```

## Discussion

The system doesn’t interpret this value; use it for whatever purpose you see fit. For example, you could store a description of the task for debugging purposes, or a key to track the task in your own data structures.

## See Also

### Obtaining general task information

var currentRequest: URLRequest?

The URL request object currently being handled by the task.

var originalRequest: URLRequest?

The original request object passed when the task was created.

var response: URLResponse?

The server’s response to the currently active request.

var taskIdentifier: Int

An identifier uniquely identifying the task within a given session.

var error: (any Error)?

An error object that indicates why the task failed.

