

- App License Delivery SDK
- ALDSession
-  generateStaticLicense(licenseID:appKey:) 

Instance Method

# generateStaticLicense(licenseID:appKey:)

Generates a static license based on the provided ALDLicenseAttribute. This method produces a static license, in a bytes array. A static license is a minimal license that is only used to install apps on the device and is not meant to enforce marketplace defined rights.

``` source
func generateStaticLicense(
    licenseID: UInt64,
    appKey: ALDAppKey
) throws
```

## Parameters 

`licenseID`  

licenseID chosen for the license

`appKey`  

The app key provided for the specified app

