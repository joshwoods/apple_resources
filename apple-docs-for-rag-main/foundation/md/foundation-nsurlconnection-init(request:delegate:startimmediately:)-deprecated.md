

- Foundation
- NSURLConnection
-  init(request:delegate:startImmediately:) Deprecated

Initializer

# init(request:delegate:startImmediately:)

Returns an initialized URL connection and begins to load the data for the URL request, if specified.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init?(
    request: URLRequest,
    delegate: Any?,
    startImmediately: Bool
)
```

Deprecated

Use NSURLSession (see NSURLSession.h)

## Parameters 

`request`  

The URL request to load. The `request` object is deep-copied as part of the initialization process. Changes made to `request` after this method returns do not affect the request that is used for the loading process.

`delegate`  

The delegate object for the connection. The connection calls methods on this delegate as the load progresses.

`startImmediately`  

true if the connection should begin loading data immediately, otherwise false. If you pass false, the connection is not scheduled with a run loop. You can then schedule the connection in the run loop and mode of your choice by calling schedule(in:forMode:).

## Return Value

The URL connection for the URL request. Returns `nil` if a connection can’t be initialized.

## Discussion

During the download the connection maintains a strong reference to the `delegate`. It releases that strong reference when the connection finishes loading, fails, or is canceled.

## See Also

### Loading Data Asynchronously

init?(request: URLRequest, delegate: Any?)

Returns an initialized URL connection and begins to load the data for the URL request.

Deprecated

class func sendAsynchronousRequest(URLRequest, queue: OperationQueue, completionHandler: (URLResponse?, Data?, (any Error)?) -> Void)

Loads the data for a URL request and executes a handler block on an operation queue when the request completes or fails.

Deprecated

func start()

Causes the connection to begin loading data, if it has not already.

