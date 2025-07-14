

- Foundation
- URLSession
- URLSession.AuthChallengeDisposition
-  URLSession.AuthChallengeDisposition.performDefaultHandling 

Case

# URLSession.AuthChallengeDisposition.performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case performDefaultHandling
```

## Mentioned in 

Performing manual server trust authentication

## See Also

### Constants

case useCredential

Use the specified credential, which may be `nil`.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

case useCredential

Use the specified credential, which may be `nil`.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

