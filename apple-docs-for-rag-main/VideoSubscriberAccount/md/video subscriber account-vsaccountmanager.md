

- Video Subscriber Account
-  VSAccountManager 

Class

# VSAccountManager

The object that coordinates your app’s authentication requests with a TV provider’s authentication service.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
class VSAccountManager
```

## Overview

The `VSAccountManager` object allows your app to request access from the user to communicate with their TV provider to understand system-level authentication status, send authentication requests for your app, and deep link to the TV Provider system settings.

## Topics

### Responding to Account Manager Requests

var delegate: (any VSAccountManagerDelegate)?

The delegate of the account manager object.

protocol VSAccountManagerDelegate

The methods you use to respond to authentication view controller requests.

### Checking Access Status

func checkAccessStatus(options: [VSCheckAccessOption : Any], completionHandler: (VSAccountAccessStatus, (any Error)?) -> Void)

Checks your app’s access to user subscription information, and requests access if needed.

struct VSCheckAccessOption

The options your app uses when checking access status.

enum VSAccountAccessStatus

Constants that represent your app’s access status to the user’s subscription information.

### Enqueuing Requests

func enqueue(VSAccountMetadataRequest, completionHandler: (VSAccountMetadata?, (any Error)?) -> Void) -> VSAccountManagerResult

Submits a request for subscriber account information.

class VSAccountMetadataRequest

An object that specifies what subscriber account information your app retrieves.

class VSAccountMetadata

A collection of information for a subscriber’s account.

class VSAccountManagerResult

An object that represents a request made for subscriber account information.

class VSAccountProviderResponse

An object that contains the response from the account provider.

struct VSAccountProviderAuthenticationScheme

Authentication schemes for account provider requests and responses.

### Deep Linking to TV Provider Settings

let VSOpenTVProviderSettingsURLString: String

A URL string you use to deep link to the system’s TV Provider settings.

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

