

- Video Subscriber Account
-  VSAccountManagerResult 

Class

# VSAccountManagerResult

An object that represents a request made for subscriber account information.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
class VSAccountManagerResult
```

## Overview

The system returns this object to your app when you app calls enqueue(_:completionHandler:). Use this object to cancel the request with cancel() while the request is in progress.

## Topics

### Cancelling a Request

func cancel()

Cancels an in-progress request for subscriber account information.

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

class VSAccountProviderResponse

An object that contains the response from the account provider.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

