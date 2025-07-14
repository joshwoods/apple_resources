

- Authentication Services
-  ASWebAuthenticationSessionRequest 

Class

# ASWebAuthenticationSessionRequest

A login session request that a web browser receives from an app.

macOS 10.15+

``` source
class ASWebAuthenticationSessionRequest
```

## Mentioned in 

Supporting Single Sign-On in a Web Browser App

## Topics

### Interpreting a Request

var url: URL

The web address the browser should use to perform the authentication request.

var callbackURLScheme: String?

The scheme the browser should use to return the result of the authentication attempt to the app requesting it.

Deprecated

var shouldUseEphemeralSession: Bool

A Boolean that indicates whether the browser should use a private browsing session.

var uuid: UUID

A unique identifier for the request.

### Finishing a Request

func complete(withCallbackURL: URL)

Indicates that the browser successfully completed the authentication attempt.

func cancelWithError(any Error)

Indicates that the browser canceled the authentication attempt.

### Indicating Completion

var delegate: (any ASWebAuthenticationSessionRequestDelegate)?

A delegate that the session request instance informs about authentication completion.

protocol ASWebAuthenticationSessionRequestDelegate

An interface through which the session request can inform its delegate, which is typically a browser, about the outcome of the authentication attempt.

### Instance Properties

var additionalHeaderFields: [String : String]?

var callback: ASWebAuthenticationSession.Callback?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Starting and Stopping a Session Request

func begin(ASWebAuthenticationSessionRequest!)

Handles the given session request from an app.

**Required**

func cancel(ASWebAuthenticationSessionRequest!)

Cancels the process of handling the given request.

**Required**

