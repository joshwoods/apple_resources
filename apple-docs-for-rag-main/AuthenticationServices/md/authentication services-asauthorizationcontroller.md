

- Authentication Services
-  ASAuthorizationController 

Class

# ASAuthorizationController

A controller that manages authorization requests that a provider creates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class ASAuthorizationController
```

## Mentioned in 

Authenticating people by using passkeys in browser apps

## Overview

Create authorization requests for the credential types your app supports, such as ASAuthorizationAppleIDRequest for Sign in with Apple, or ASAuthorizationPasswordRequest for password credentials. Create an authorization controller using init(authorizationRequests:), supplying the authorization requests you create. Set the authorization controller’s delegate to receive responses when requests succeed or fail, and set its presentationContextProvider so that the authorization controller can present UI.

Call performAutoFillAssistedRequests() to present inline UI to request credentials, or performRequests() or performRequests(options:) to request credentials using modal UI. ASAuthorizationController calls your delegate’s methods when the request completes.

Set the content type of text fields in your app’s login UI so that ASAuthorizationController can detect when to offer AutoFill suggestions. Use username as the content type for user name text fields, and password for password fields.

## Topics

### Creating a controller

init(authorizationRequests: [ASAuthorizationRequest])

Creates a controller from a collection of authorization requests.

### Inspecting requests

class ASAuthorizationRequest

A base class for different kinds of authorization requests.

var authorizationRequests: [ASAuthorizationRequest]

The authorization requests that the controller manages.

var customAuthorizationMethods: [ASAuthorizationCustomMethod]

An array of custom authorization methods for the user to choose.

### Presenting requests

var presentationContextProvider: (any ASAuthorizationControllerPresentationContextProviding)?

A delegate that provides a display context in which the system can present an authorization interface to the user.

protocol ASAuthorizationControllerPresentationContextProviding

An interface the controller uses to ask a delegate for a presentation context.

### Executing requests

func performRequests()

Starts the specified authorization flows during controller initialization.

func performRequests(options: ASAuthorizationController.RequestOptions)

Starts the specified authorization flows during controller initialization.

func performAutoFillAssistedRequests()

Initiates the authorization flows for requests that support AutoFill presentation.

func cancel()

Cancels any active authorization requests.

struct RequestOptions

Options that modify how a controller performs authorization requests.

### Responding to request completion

var delegate: (any ASAuthorizationControllerDelegate)?

A delegate that the authorization controller informs about the success or failure of an authorization attempt.

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

protocol ASAuthorizationControllerDelegate

An interface for providing information about the outcome of an authorization request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Authorization requests

struct AuthorizationController

A SwiftUI environment value that views use to perform authorization requests.

enum ASAuthorizationResult

Describes the outcome of a successful authorization request.

