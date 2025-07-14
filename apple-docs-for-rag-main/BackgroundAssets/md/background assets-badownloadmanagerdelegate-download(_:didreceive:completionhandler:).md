

- Background Assets
- BADownloadManagerDelegate
-  download(\_:didReceive:completionHandler:) 

Instance Method

# download(\_:didReceive:completionHandler:)

Tells the delegate to resolve the specified URL authentication challenge.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
optional func download(
    _ download: BADownload,
    didReceive challenge: URLAuthenticationChallenge,
    completionHandler: @escaping (URLSession.AuthChallengeDisposition, URLCredential?) -> Void
)
```

``` source
optional func download(
    _ download: BADownload,
    didReceive challenge: URLAuthenticationChallenge
) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

## Parameters 

`download`  

The associated asset download.

`challenge`  

An object that provides the information you need to decide how to respond to the server’s request for authentication.

`completionHandler`  

The completion handler you call to tell the system how to respond to the challenge.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as this page explains, or you can call it as an asynchronous method that has the following declaration:

```
optional func download(_ download: BADownload, didReceive challenge: URLAuthenticationChallenge) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The completion handler takes the following parameters:

- An URLSession.AuthChallengeDisposition that indicates whether the system processes, cancels, or rejects the challenge.

- If the specified dispostion is URLSession.AuthChallengeDisposition.useCredential, the URLCredential to use for authentication; otherwise, specify `nil`.

If you implement this method, make sure to call the completion handler promptly and with the necessary information. Otherwise, the server may deny the request and the associated asset download fails.

For more information about authentication challenges, see Handling an authentication challenge.

## See Also

### Reacting to download events

func downloadDidBegin(BADownload)

Informs the delegate about a started asset download.

func download(BADownload, didWriteBytes: Int64, totalBytesWritten: Int64, totalBytesExpectedToWrite: Int64)

Informs the delegate about the progress of the specified asset download.

func downloadDidPause(BADownload)

Informs the delegate about a paused asset download.

