

- Foundation
- URLSession
-  dataTaskPublisher(for:) 

Instance Method

# dataTaskPublisher(for:)

Returns a publisher that wraps a URL session data task for a given URL request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dataTaskPublisher(for request: URLRequest) -> URLSession.DataTaskPublisher
```

## Parameters 

`request`  

The URL request for which to create a data task.

## Discussion

The publisher publishes data when the task completes, or terminates if the task fails with an error.

## See Also

### Performing tasks as a Combine Publisher

Processing URL session data task results with Combine

Use a chain of asynchronous operators to receive and process data fetched from a URL.

func dataTaskPublisher(for: URL) -> URLSession.DataTaskPublisher

Returns a publisher that wraps a URL session data task for a given URL.

struct DataTaskPublisher

A publisher that delivers the results of performing URL session data tasks.

