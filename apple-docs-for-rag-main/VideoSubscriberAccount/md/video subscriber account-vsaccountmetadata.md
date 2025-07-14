

- Video Subscriber Account
-  VSAccountMetadata 

Class

# VSAccountMetadata

A collection of information for a subscriber’s account.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
class VSAccountMetadata
```

## Overview

The VSAccountMetadata object contains the information you requested in the VSAccountMetadataRequest object that you passed to the enqueue(_:completionHandler:) method. If the call succeeds, the system sends the VSAccountMetadata object to your app’s completion handler for your app to process.

## Topics

### Getting TV Provider Info

var accountProviderIdentifier: String?

The unique identifier of the account provider.

var authenticationExpirationDate: Date?

The date when the user’s current authentication session expires.

### Getting App Authentication Info

var accountProviderResponse: VSAccountProviderResponse?

The response from the account provider.

var samlAttributeQueryResponse: String?

The SAML response from the account provider.

var verificationData: Data?

Data you use to verify that the response came from the account provider.

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

class VSAccountMetadataRequest

An object that specifies what subscriber account information your app retrieves.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

class VSAccountProviderResponse

An object that contains the response from the account provider.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

