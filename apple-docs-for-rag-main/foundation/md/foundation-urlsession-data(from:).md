

- Foundation
- URLSession
-  data(from:) 

Instance Method

# data(from:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func data(from url: URL) async throws -> (Data, URLResponse)
```

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

func download(for: URLRequest, delegate: (any URLSessionTaskDelegate)?) async throws -> (URL, URLResponse)

Retrieves the contents of a URL based on the specified URL request and delivers the URL of the saved file asynchronously.

func download(from: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (URL, URLResponse)

Retrieves the contents of a URL and delivers the URL of the saved file asynchronously.

func download(resumeFrom: Data, delegate: (any URLSessionTaskDelegate)?) async throws -> (URL, URLResponse)

Resumes a previously-paused download and delivers the URL of the saved file asynchronously.

func upload(for: URLRequest, from: Data, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Uploads data to a URL based on the specified URL request and delivers the result asynchronously.

func upload(for: URLRequest, fromFile: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (Data, URLResponse)

Uploads data to a URL and delivers the result asynchronously.

func upload(for: URLRequest, from: Data) async throws -> (Data, URLResponse)

func upload(for: URLRequest, fromFile: URL) async throws -> (Data, URLResponse)

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

