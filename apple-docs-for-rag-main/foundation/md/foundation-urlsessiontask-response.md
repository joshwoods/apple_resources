

- Foundation
- URLSessionTask
-  response 

Instance Property

# response

The server’s response to the currently active request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var response: URLResponse? { get }
```

## Mentioned in 

Downloading files from websites

## Discussion

This object provides information about the request as provided by the server. This information always includes the original URL. It may also include an expected length, MIME type information, encoding information, a suggested filename, or a combination of these.

## See Also

### Obtaining general task information

var currentRequest: URLRequest?

The URL request object currently being handled by the task.

var originalRequest: URLRequest?

The original request object passed when the task was created.

var taskDescription: String?

An app-provided string value for the current task.

var taskIdentifier: Int

An identifier uniquely identifying the task within a given session.

var error: (any Error)?

An error object that indicates why the task failed.

