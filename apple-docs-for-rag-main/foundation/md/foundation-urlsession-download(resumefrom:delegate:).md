

- Foundation
- URLSession
-  download(resumeFrom:delegate:) 

Instance Method

# download(resumeFrom:delegate:)

Resumes a previously-paused download and delivers the URL of the saved file asynchronously.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func download(
    resumeFrom resumeData: Data,
    delegate: (any URLSessionTaskDelegate)? = nil
) async throws -> (URL, URLResponse)
```

## Parameters 

`resumeData`  

A data object that provides the data necessary to resume a download.

`delegate`  

A delegate that receives life cycle and authentication challenge callbacks as the transfer progresses.

## Return Value

An asynchronously-delivered tuple that contains the location of the downloaded file as a URL, and a URLResponse.

## Discussion

Your app can obtain a `resumeData` object in two ways:

- If your app cancels an existing transfer by calling cancel(byProducingResumeData:), the session object passes a `resumeData` object to the completion handler that you provided in that call.

- If a transfer fails, the session object provides an `NSError` object either to its delegate or to the task’s completion handler. In that object, the NSURLSessionDownloadTaskResumeData key in the `userInfo` dictionary contains a `resumeData` object.

## See Also

### Performing asynchronous transfers

func bytes(for: URLRequest, delegate: (any URLSessionTaskDelegate)?) async throws -> (URLSession.AsyncBytes, URLResponse)

Retrieves the contents of a URL based on the specified URL request and delivers an asynchronous sequence of bytes.

func bytes(from: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (URLSession.AsyncBytes, URLResponse)

Retrieves the contents of a given URL and delivers an asynchronous sequence of bytes.

struct AsyncBytes

An asynchronous sequence of bytes.

func data(for: URLRequest, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Downloads the contents of a URL based on the specified URL request and delivers the data asynchronously.

func data(from: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Retrieves the contents of a URL and delivers the data asynchronously.

func data(for: URLRequest) async throws -> (Data, URLResponse)

func data(from: URL) async throws -> (Data, URLResponse)

func download(for: URLRequest, delegate: (any URLSessionTaskDelegate)?) async throws -> (URL, URLResponse)

Retrieves the contents of a URL based on the specified URL request and delivers the URL of the saved file asynchronously.

func download(from: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (URL, URLResponse)

Retrieves the contents of a URL and delivers the URL of the saved file asynchronously.

func upload(for: URLRequest, from: Data, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Uploads data to a URL based on the specified URL request and delivers the result asynchronously.

func upload(for: URLRequest, fromFile: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Uploads data to a URL and delivers the result asynchronously.

func upload(for: URLRequest, from: Data) async throws -> (Data, URLResponse)

func upload(for: URLRequest, fromFile: URL) async throws -> (Data, URLResponse)

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

