

- Video Subscriber Account
-  VSAccountMetadataRequest 

Class

# VSAccountMetadataRequest

An object that specifies what subscriber account information your app retrieves.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
class VSAccountMetadataRequest
```

## Overview

Use a `VSAccountMetadataRequest` object to indicate the specific information your app will obtain about a subscriber from their subscription provider. Also, use this object to provide information to the subscription provider that it needs to perform the request, such as a verification token, the authentication schemes your app supports, or your app’s identifier.

## Topics

### Requesting TV Provider Info

var includeAccountProviderIdentifier: Bool

A Boolean value that indicates whether your app requests the identifier of the account provider.

var includeAuthenticationExpirationDate: Bool

A Boolean value that indicates whether your app requests the expiration date of the user’s current authentication session.

### Requesting App-Level Authentication

var attributeNames: [String]

The SAML attributes that your app sends to the account provider.

var channelIdentifier: String?

The channel identifier for the request.

var supportedAccountProviderIdentifiers: [String]

A list of identifiers for TV providers that your app supports.

var supportedAuthenticationSchemes: [VSAccountProviderAuthenticationScheme]

A collection of authentication schemes your app supports for this request.

var verificationToken: String?

A token that your app sends to an account provider to identify itself.

### Specifying Additional Options

var isInterruptionAllowed: Bool

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

var featuredAccountProviderIdentifiers: [String]

The providers your app lists prominently during authentication.

var forceAuthentication: Bool

A Boolean value that indicates whether the app ignores cached credentials.

var localizedVideoTitle: String?

A short, user-presentable name for the video that the user wants to play.

var applicationAccountProviders: [VSAccountApplicationProvider]?

An array of application-specific providers to add to the list of account providers.

### Supporting Authentication Share

var accountProviderAuthenticationToken: String?

An authentication session token that your app sends to the account provider.

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

### Enqueuing Requests

func enqueue(VSAccountMetadataRequest, completionHandler: (VSAccountMetadata?, (any Error)?) -> Void) -> VSAccountManagerResult

Submits a request for subscriber account information.

class VSAccountMetadata

A collection of information for a subscriber’s account.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

class VSAccountProviderResponse

An object that contains the response from the account provider.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

