

- Foundation
- URLCredential
-  init(forTrust:) 

Initializer

# init(forTrust:)

Creates a URL credential instance for server trust authentication with a given accepted trust.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(forTrust trust: SecTrust)
```

## Parameters 

`trust`  

The accepted trust.

## Return Value

A new URL credential object, containing the accepted server trust.

## Discussion

Before creating a server trust credential, it is the responsibility of the delegate of an NSURLConnection instance or an NSURLDownload instance to evaluate the trust. Do this by calling SecTrustEvaluate(_:_:), passing it the trust obtained from the `serverTrust` method of the server’s URLProtectionSpace instance. If the trust is invalid, the authentication challenge should be cancelled with cancel(_:).

## See Also

### Creating a credential

init(identity: SecIdentity, certificates: [Any]?, persistence: URLCredential.Persistence)

Creates a URL credential instance for resolving a client certificate authentication challenge.

init(trust: SecTrust)

Creates a URL credential instance for server trust authentication, initialized with a accepted trust.

init(user: String, password: String, persistence: URLCredential.Persistence)

Creates a URL credential instance initialized with a given user name and password, using a given persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

