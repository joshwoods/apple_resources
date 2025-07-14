

- App License Delivery SDK
-  ALDLicenseAttribute 

Structure

# ALDLicenseAttribute

A structure that defines the requested license type for the session.

``` source
struct ALDLicenseAttribute
```

## Topics

### Initializers

init(licenseID: UInt64)

Create a license attribue

### Instance Properties

var duration: UInt64

The maximum amount of time, in seconds, that iOS considers the license valid.

var issuedTime: UInt64

### Instance Methods

func addAppKey(ALDAppKey) throws

Add an AppKey to be associated with this license

func revokeAppleItemID(UInt64) throws

An appleItemID to be revoked by the license

## See Also

### App licensing

Licensing alternative distribution apps

Build a license server that supports the installation of your apps and the apps available in your marketplace.

Renewing and revoking app licenses

Determine whether an app for which you issue a license launches.

struct ALDAppKey

A structure that identifies an app and a key that’s required to decrypt the app’s license request.

class ALDProvider

An object that creates a session with the alternative app marketplace’s signing assets.

class ALDSession

A structure that contains the details of a license request and methods to generate license responses.

