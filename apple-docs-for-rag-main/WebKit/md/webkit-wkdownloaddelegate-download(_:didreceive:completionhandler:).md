

- WebKit
- WKDownloadDelegate
-  download(\_:didReceive:completionHandler:) 

Instance Method

# download(\_:didReceive:completionHandler:)

Asks the delegate to respond to an authentication challenge.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    didReceive challenge: URLAuthenticationChallenge,
    completionHandler: @escaping @MainActor (URLSession.AuthChallengeDisposition, URLCredential?) -> Void
)
```

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    respondTo challenge: URLAuthenticationChallenge
) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

## Parameters 

`download`  

The download that received the authentication challenge.

`challenge`  

The authentication challenge.

`completionHandler`  

A closure you must invoke to respond to the authentication challenge. Provide the closure with a disposition that describes how to respond to the authorization challenge, and optional credentials.

## Discussion

Determine how to respond to the authentication challenge in this method. Then invoke `completionHandler` with a disposition that describes how to respond to the authorization challenge, and optional credentials.

If you don’t implement this method, the web view responds to the challenge with URLSession.AuthChallengeDisposition.rejectProtectionSpace.

## See Also

### Responding to Authorization Challenges

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

