

- StoreKit
- SKCloudServiceController
-  authorizationStatus() Deprecated

Type Method

# authorizationStatus()

Returns the type of authorization the customer has for accessing the Music library on the device.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
class func authorizationStatus() -> SKCloudServiceAuthorizationStatus
```

Deprecated

Use MusicAuthorization.currentStatus from MusicKit

## Return Value

The type of authorization for music library access. See SKCloudServiceAuthorizationStatus for a list of possible values.

## Mentioned in 

Requesting Access to Apple Music Library

Determining a person’s Apple Music capabilities

Offering Apple Music Subscription in Your App

## Discussion

Use the authorization status to determine in what ways you can access the user’s music library.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Getting authorization to access the Music library

Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

class func requestAuthorization((SKCloudServiceAuthorizationStatus) -> Void)

Asks the customer for permission to access the Music library on the device.

Deprecated

enum SKCloudServiceAuthorizationStatus

Constants that indicate the type of authorization the customer has for accessing the Music library.

Deprecated

