

- Foundation
- URLSessionTaskDelegate
-  urlSession(\_:task:needNewBodyStreamFrom:completionHandler:) 

Instance Method

# urlSession(\_:task:needNewBodyStreamFrom:completionHandler:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
optional func urlSession(
    _ session: URLSession,
    task: URLSessionTask,
    needNewBodyStreamFrom offset: Int64,
    completionHandler: @escaping (InputStream?) -> Void
)
```

``` source
optional func urlSession(
    _ session: URLSession,
    needNewBodyStreamForTask task: URLSessionTask,
    from offset: Int64
) async -> InputStream?
```

