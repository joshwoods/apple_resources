

- Foundation
- NSURLConnection
-  sendAsynchronousRequest(\_:queue:completionHandler:) Deprecated

Type Method

# sendAsynchronousRequest(\_:queue:completionHandler:)

Loads the data for a URL request and executes a handler block on an operation queue when the request completes or fails.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
class func sendAsynchronousRequest(
    _ request: URLRequest,
    queue: OperationQueue,
    completionHandler handler: @escaping (URLResponse?, Data?, (any Error)?) -> Void
)
```

**Mac Catalyst, visionOS**

``` source
class func sendAsynchronousRequest(
    _ request: URLRequest,
    queue: OperationQueue
) async throws -> (URLResponse, Data)
```

Deprecated

Use \[NSURLSession dataTaskWithRequest:completionHandler:\] (see NSURLSession.h

## Parameters 

`request`  

The URL request to load. The `request` object is deep-copied as part of the initialization process. Changes made to `request` after this method returns do not affect the request that is used for the loading process.

`queue`  

The operation queue to which the handler block is dispatched when the request completes or failed.

`handler`  

The handler block to execute.

## Discussion

If the request completes successfully, the `data` parameter of the handler block contains the resource data, and the `error` parameter is `nil`. If the request fails, the `data` parameter is `nil` and the error parameter contain information about the failure.

If authentication is required in order to download the request, the required credentials must be specified as part of the URL. If authentication fails, or credentials are missing, the connection will attempt to continue without credentials. If the request finishes with a `401 Unauthorized` status code, the `response` parameter is `nil`, the `data` parameter contains the resource data, and the `error` parameter is an `NSError` with the NSURLErrorUserCancelledAuthentication code in the NSURLErrorDomain error domain.

## See Also

### Loading Data Asynchronously

init?(request: URLRequest, delegate: Any?)

Returns an initialized URL connection and begins to load the data for the URL request.

Deprecated

init?(request: URLRequest, delegate: Any?, startImmediately: Bool)

Returns an initialized URL connection and begins to load the data for the URL request, if specified.

Deprecated

func start()

Causes the connection to begin loading data, if it has not already.

