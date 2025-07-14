

- Foundation
- URLSession
- URLSession.AuthChallengeDisposition
-  URLSession.AuthChallengeDisposition.useCredential 

Case

# URLSession.AuthChallengeDisposition.useCredential

Use the specified credential, which may be `nil`.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case useCredential
```

## Mentioned in 

Performing manual server trust authentication

## See Also

### Constants

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

