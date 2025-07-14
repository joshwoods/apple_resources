

- App License Delivery SDK
-  ALDProvider 

Class

# ALDProvider

An object that creates a session with the alternative app marketplace’s signing assets.

``` source
class ALDProvider
```

## Mentioned in 

Licensing alternative distribution apps

## Topics

### Initializers

init(encryptionCert: [UInt8], signingCert: [UInt8], PASK: [UInt8], signingKey: [UInt8]?)

Initializes a provider with the marketplace’s App License Delivery assets and their unique signing key.

### Instance Methods

func createSession(clientRequest: [UInt8]) throws -> ALDSession

Creates an ALD Session

## See Also

### App licensing

Licensing alternative distribution apps

Build a license server that supports the installation of your apps and the apps available in your marketplace.

Renewing and revoking app licenses

Determine whether an app for which you issue a license launches.

struct ALDAppKey

A structure that identifies an app and a key that’s required to decrypt the app’s license request.

struct ALDLicenseAttribute

A structure that defines the requested license type for the session.

class ALDSession

A structure that contains the details of a license request and methods to generate license responses.

