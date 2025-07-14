

- Video Subscriber Account
-  VSAccountProviderResponse 

Class

# VSAccountProviderResponse

An object that contains the response from the account provider.

iOS 10.2+iPadOS 10.2+macOStvOS 10.1+visionOS 1.0+

``` source
class VSAccountProviderResponse
```

## Overview

A `VSAccountProviderResponse` object encapsulates the information the account provider sends back to your app, such as authentication scheme type, raw response data, and status code.

## Topics

### Getting Response Info

var authenticationScheme: VSAccountProviderAuthenticationScheme

The authentication scheme type of the response.

var body: String?

The raw response from the provider.

var status: String?

The status code for the response.

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

class VSAccountMetadata

A collection of information for a subscriber’s account.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

