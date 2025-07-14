

- Foundation
- URLSession
-  URLSession.AuthChallengeDisposition 

Enumeration

# URLSession.AuthChallengeDisposition

Constants passed by session or task delegates to the provided continuation block in response to an authentication challenge.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum AuthChallengeDisposition
```

## Topics

### Constants

case useCredential

Use the specified credential, which may be `nil`.

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

case useCredential

Use the specified credential, which may be `nil`.

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling authentication challenges

func urlSession(URLSession, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Requests credentials from the delegate in response to a session-level authentication request from the remote server.

