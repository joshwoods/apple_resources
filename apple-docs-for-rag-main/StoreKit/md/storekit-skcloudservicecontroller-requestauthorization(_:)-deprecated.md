

- StoreKit
- SKCloudServiceController
-  requestAuthorization(\_:) Deprecated

Type Method

# requestAuthorization(\_:)

Asks the customer for permission to access the Music library on the device.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
class func requestAuthorization(_ completionHandler: @escaping (SKCloudServiceAuthorizationStatus) -> Void)
```

``` source
class func requestAuthorization() async -> SKCloudServiceAuthorizationStatus
```

Deprecated

Use MusicAuthorization.request() from MusicKit

## Parameters 

`completionHandler`  

A block that is called when authorization is granted or denied by the user.

## Mentioned in 

Requesting Access to Apple Music Library

Determining a person’s Apple Music capabilities

## Discussion

You can use this method to ask the user for permission to play Apple Music tracks or to add tracks to the music library.

## See Also

### Getting authorization to access the Music library

Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

class func authorizationStatus() -> SKCloudServiceAuthorizationStatus

Returns the type of authorization the customer has for accessing the Music library on the device.

Deprecated

enum SKCloudServiceAuthorizationStatus

Constants that indicate the type of authorization the customer has for accessing the Music library.

Deprecated

