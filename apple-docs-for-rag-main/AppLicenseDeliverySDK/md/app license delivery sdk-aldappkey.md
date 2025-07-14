

- App License Delivery SDK
-  ALDAppKey 

Structure

# ALDAppKey

A structure that identifies an app and a key that’s required to decrypt the app’s license request.

``` source
struct ALDAppKey
```

## Overview

An instance of this structure represents a unique variant for an app. The AppleItemID argument to the init(appleItemID:appKeyBlob:) initializer refers to the app, and the `appKeyBlob` argument refers to a *key blob* for a specific app variant that App Store Connect provides your marketplace server during app ingestion. For more information, see Ingesting an alternative distribution package.

## Topics

### Initializers

init(appleItemID: UInt64, appKeyBlob: [UInt8]) throws

Creates an app key to decrypt a license request.

## See Also

### App licensing

Licensing alternative distribution apps

Build a license server that supports the installation of your apps and the apps available in your marketplace.

Renewing and revoking app licenses

Determine whether an app for which you issue a license launches.

struct ALDLicenseAttribute

A structure that defines the requested license type for the session.

class ALDProvider

An object that creates a session with the alternative app marketplace’s signing assets.

class ALDSession

A structure that contains the details of a license request and methods to generate license responses.

