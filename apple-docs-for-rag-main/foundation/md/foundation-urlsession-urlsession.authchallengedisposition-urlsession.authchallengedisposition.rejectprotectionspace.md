

- Foundation
- URLSession
- URLSession.AuthChallengeDisposition
-  URLSession.AuthChallengeDisposition.rejectProtectionSpace 

Case

# URLSession.AuthChallengeDisposition.rejectProtectionSpace

Reject this challenge, and call the authentication delegate method again with the next authentication protection space. The provided credential parameter is ignored.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case rejectProtectionSpace
```

## Discussion

The URLSession.AuthChallengeDisposition.rejectProtectionSpace disposition is only appropriate in fairly unusual situations. For example, a Windows server might use both NSURLAuthenticationMethodNegotiate and NSURLAuthenticationMethodNTLM. If your app can only handle NTLM, you would want to reject the Negotiate challenge, in order to then receive the queued NTLM challenge.

However, most apps won’t face this scenario, and if you cannot provide a credential for a certain authentication method, you should usually fall back to the URLSession.AuthChallengeDisposition.performDefaultHandling disposition instead.

## See Also

### Constants

case useCredential

Use the specified credential, which may be `nil`.

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

case useCredential

Use the specified credential, which may be `nil`.

case performDefaultHandling

Use the default handling for the challenge as though this delegate method were not implemented. The provided credential parameter is ignored.

case cancelAuthenticationChallenge

Cancel the entire request. The provided credential parameter is ignored.

