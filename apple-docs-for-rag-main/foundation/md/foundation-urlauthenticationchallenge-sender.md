

- Foundation
- URLAuthenticationChallenge
-  sender 

Instance Property

# sender

The sender of the challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sender: (any URLAuthenticationChallengeSender)? { get }
```

## Discussion

If you are using the URLSession API, this value is purely informational, because you *must* respond to authentication challenges in your URLSessionDelegate or URLSessionTaskDelegate implementations, by passing URLSession.AuthChallengeDisposition constants to the provided completion handler blocks.

However, if you are using the legacy `NSURLConnection` or `NSURLDownload` API, you use this object directly in your authentication handler delegate method. With these APIs, after you finish processing the authentication challenge, you respond by calling methods defined in the URLAuthenticationChallengeSender protocol on this sender.

Warning

Do not call methods directly on this object if you are using the URLSession API.

