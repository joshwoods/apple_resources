

- Foundation
- URLCredential
-  init(trust:) 

Initializer

# init(trust:)

Creates a URL credential instance for server trust authentication, initialized with a accepted trust.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(trust: SecTrust)
```

## Parameters 

`trust`  

The accepted trust.

## Return Value

A new URL credential object, containing the provided server trust.

## Discussion

Before your implementation of urlSession(_:task:didReceive:completionHandler:) uses this initializer to create a server trust credential, you are responsible for evaluating the received SecTrust instance. You get this serverTrust from the protectionSpace of the URLAuthenticationChallenge parameter that is passed to your delegate method. Pass the trust instance to SecTrustEvaluate(_:_:) to evaluate it. If this call indicates the trust is invalid, you should cancel the challenge by passing the URLSession.AuthChallengeDisposition.cancelAuthenticationChallenge disposition to the completion handler.

## See Also

### Creating a credential

init(forTrust: SecTrust)

Creates a URL credential instance for server trust authentication with a given accepted trust.

init(identity: SecIdentity, certificates: [Any]?, persistence: URLCredential.Persistence)

Creates a URL credential instance for resolving a client certificate authentication challenge.

init(user: String, password: String, persistence: URLCredential.Persistence)

Creates a URL credential instance initialized with a given user name and password, using a given persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

