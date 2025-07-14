

- Foundation
- URLAuthenticationChallenge
-  init(authenticationChallenge:sender:) 

Initializer

# init(authenticationChallenge:sender:)

Creates an authentication challenge from an existing challenge instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    authenticationChallenge challenge: URLAuthenticationChallenge,
    sender: any URLAuthenticationChallengeSender
)
```

## Parameters 

`challenge`  

The challenge that you want to copy. Usually, this is a challenge received by an existing URLProtocol subclass that you are subclassing.

`sender`  

The sender that you want to use for the new object. Typically, the sender is the instance of your custom URLProtocol subclass that called this method.

## Return Value

A new authentication challenge object, based on an existing challenge.

## Discussion

Most apps don’t create URLAuthenticationChallenge instances themselves. Instead, they handle received challenges in the urlSession(_:task:didReceive:completionHandler:) method of URLSessionTaskDelegate.

However, you might need to create authentication challenge objects when adding support for custom networking protocols, as part of a custom URLProtocol subclass. When you subclass an existing URLProtocol subclass, this initializer lets you modify challenges issued by the existing class so that your subclass receives any responses to those challenges.

## See Also

### Creating an authentication challenge instance

init(protectionSpace: URLProtectionSpace, proposedCredential: URLCredential?, previousFailureCount: Int, failureResponse: URLResponse?, error: (any Error)?, sender: any URLAuthenticationChallengeSender)

Initializes an authentication challenge from parameters you provide.

