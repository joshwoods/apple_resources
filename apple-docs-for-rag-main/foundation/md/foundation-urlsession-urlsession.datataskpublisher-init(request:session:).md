

- Foundation
- URLSession
- URLSession.DataTaskPublisher
-  init(request:session:) 

Initializer

# init(request:session:)

Creates a data task publisher from the provided URL request and URL session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    request: URLRequest,
    session: URLSession
)
```

## Parameters 

`request`  

The URLRequest from which to create a URL session data task.

`session`  

The URLSession to create the data task.

