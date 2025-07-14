

- Foundation
- URLSession
-  URLSession.DataTaskPublisher 

Structure

# URLSession.DataTaskPublisher

A publisher that delivers the results of performing URL session data tasks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct DataTaskPublisher
```

## Mentioned in 

Processing URL session data task results with Combine

## Topics

### Creating a data task publisher

init(request: URLRequest, session: URLSession)

Creates a data task publisher from the provided URL request and URL session.

### Inspecting data task properties

let request: URLRequest

The URL request performed by the data task associated with this publisher.

let session: URLSession

The URL session that performs the data task associated with this publisher.

## Relationships

### Conforms To

- Publisher
- Sendable

## See Also

### Performing tasks as a Combine Publisher

Processing URL session data task results with Combine

Use a chain of asynchronous operators to receive and process data fetched from a URL.

func dataTaskPublisher(for: URLRequest) -> URLSession.DataTaskPublisher

Returns a publisher that wraps a URL session data task for a given URL request.

func dataTaskPublisher(for: URL) -> URLSession.DataTaskPublisher

Returns a publisher that wraps a URL session data task for a given URL.

