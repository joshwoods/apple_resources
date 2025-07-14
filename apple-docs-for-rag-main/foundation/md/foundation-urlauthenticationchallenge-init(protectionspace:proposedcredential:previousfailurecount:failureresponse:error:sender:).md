

- Foundation
- URLAuthenticationChallenge
-  init(protectionSpace:proposedCredential:previousFailureCount:failureResponse:error:sender:) 

Initializer

# init(protectionSpace:proposedCredential:previousFailureCount:failureResponse:error:sender:)

Initializes an authentication challenge from parameters you provide.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    protectionSpace space: URLProtectionSpace,
    proposedCredential credential: URLCredential?,
    previousFailureCount: Int,
    failureResponse response: URLResponse?,
    error: (any Error)?,
    sender: any URLAuthenticationChallengeSender
)
```

## Parameters 

`space`  

The protection space for the authentication challenge. This provides additional information about the authentication request, such as the host, port, authentication realm, and so on.

`credential`  

The proposed credential, or `nil`.

`previousFailureCount`  

The total number of previous failures for this request, including failures for other protection spaces.

`response`  

An instance of URLResponse containing the server response that caused you to generate an authentication challenge, or `nil` if no response object is applicable to the challenge.

`error`  

An ``` NS``Error ``` instance describing the authentication failure, or `nil` if it is not applicable to the challenge.

`sender`  

The object that initiated the authentication challenge (typically, the object that called this method).

## Return Value

A new authentication challenge object, with the given properties.

## Discussion

Most apps don’t create URLAuthenticationChallenge instances themselves. Instead, they handle received challenges in the urlSession(_:task:didReceive:completionHandler:) method of URLSessionTaskDelegate.

However, you might need to create authentication challenge objects when adding support for custom networking protocols, as part of your custom URLProtocol subclasses.

## See Also

### Creating an authentication challenge instance

init(authenticationChallenge: URLAuthenticationChallenge, sender: any URLAuthenticationChallengeSender)

Creates an authentication challenge from an existing challenge instance.

