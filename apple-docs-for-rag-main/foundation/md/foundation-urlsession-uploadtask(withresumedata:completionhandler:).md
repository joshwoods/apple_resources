

- Foundation
- URLSession
-  uploadTask(withResumeData:completionHandler:) 

Instance Method

# uploadTask(withResumeData:completionHandler:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func uploadTask(
    withResumeData resumeData: Data,
    completionHandler: @escaping (Data?, URLResponse?, (any Error)?) -> Void
) -> URLSessionUploadTask
```

## See Also

### Adding upload tasks to a session

func uploadTask(with: URLRequest, from: Data) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object and uploads the provided data.

func uploadTask(with: URLRequest, from: Data?, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

Creates a task that performs an HTTP request for the specified URL request object, uploads the provided data, and calls a handler upon completion.

func uploadTask(with: URLRequest, fromFile: URL) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading the specified file.

func uploadTask(with: URLRequest, fromFile: URL, completionHandler: (Data?, URLResponse?, (any Error)?) -> Void) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading the specified file, then calls a handler upon completion.

func uploadTask(withStreamedRequest: URLRequest) -> URLSessionUploadTask

Creates a task that performs an HTTP request for uploading data based on the specified URL request.

func uploadTask(withResumeData: Data) -> URLSessionUploadTask

class URLSessionUploadTask

A URL session task that uploads data to the network in a request body.

protocol URLSessionDataDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to data and upload tasks.

