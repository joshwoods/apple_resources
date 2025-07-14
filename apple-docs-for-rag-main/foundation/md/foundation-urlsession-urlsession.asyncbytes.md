

- Foundation
- URLSession
-  URLSession.AsyncBytes 

Structure

# URLSession.AsyncBytes

An asynchronous sequence of bytes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AsyncBytes
```

## Topics

### Adapting textual sequences

struct AsyncCharacterSequence

An asynchronous sequence of characters.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

struct AsyncLineSequence

An asynchronous sequence of lines of text.

### Accessing the URL session task

var task: URLSessionDataTask

The URL session task that performs the data transfer.

### Structures

struct Iterator

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Performing asynchronous transfers

func bytes(for: URLRequest, delegate: (any URLSessionTaskDelegate)?) async throws -> (URLSession.AsyncBytes, URLResponse)

Retrieves the contents of a URL based on the specified URL request and delivers an asynchronous sequence of bytes.

func bytes(from: URL, delegate: (any URLSessionTaskDelegate)?) async throws -> (URLSession.AsyncBytes, URLResponse)

Retrieves the contents of a given URL and delivers an asynchronous sequence of bytes.

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

