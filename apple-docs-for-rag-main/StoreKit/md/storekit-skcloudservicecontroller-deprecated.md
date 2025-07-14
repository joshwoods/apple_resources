

- StoreKit
-  SKCloudServiceController Deprecated

Class

# SKCloudServiceController

An object that determines the current capabilities of a person’s Music library.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
class SKCloudServiceController
```

Deprecated

Use SwiftUI and MusicKit instead.

## Mentioned in 

Determining a person’s Apple Music capabilities

Requesting Access to Apple Music Library

Offering Apple Music Subscription in Your App

## Overview

Use an SKCloudServiceController object to determine the current capabilities of a customer’s Music library, like whether the device allows playback of Apple Music catalog tracks and the addition of tracks to the library.

## Topics

### Getting authorization to access the Music library

Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

class func authorizationStatus() -> SKCloudServiceAuthorizationStatus

Returns the type of authorization the customer has for accessing the Music library on the device.

class func requestAuthorization((SKCloudServiceAuthorizationStatus) -> Void)

Asks the customer for permission to access the Music library on the device.

enum SKCloudServiceAuthorizationStatus

Constants that indicate the type of authorization the customer has for accessing the Music library.

### Determining capabilities

Determining a person’s Apple Music capabilities

Determine which Apple Music capabilities are available on a customer’s device.

func requestUserToken(forDeveloperToken: String, completionHandler: (String?, (any Error)?) -> Void)

Returns a user token that you use to access personalized Apple Music content.

func requestStorefrontCountryCode(completionHandler: (String?, (any Error)?) -> Void)

Gets the country code for the storefront associated with a customer’s iTunes account.

func requestCapabilities(completionHandler: (SKCloudServiceCapability, (any Error)?) -> Void)

Gets the current capabilities associated with the Music library on the device.

struct SKCloudServiceCapability

Constants that specify the current capabilities of the customer’s Music library on the device.

func requestStorefrontIdentifier(completionHandler: (String?, (any Error)?) -> Void)

Gets the device’s storefront identifier.

func requestPersonalizationToken(forClientToken: String, withCompletionHandler: (String?, (any Error)?) -> Void)

### Notifications

static let SKStorefrontIdentifierDidChange: NSNotification.Name

A notification name for indicating a change in the storefront identifier associated with the device.

static let SKCloudServiceCapabilitiesDidChange: NSNotification.Name

A notification name for indicating a change in the capabilities associated with the Music library on the device.

static let SKStorefrontCountryCodeDidChange: NSNotification.Name

A notification name for indicating a change in the storefront country or region code associated with the device.

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

### Deprecated

class SKCloudServiceSetupViewController

A view controller that helps people perform setup for a cloud service, like an Apple Music subscription.

Deprecated

