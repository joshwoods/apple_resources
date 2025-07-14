

- App License Delivery SDK
- ALDSession
-  generateLicense(attr:) 

Instance Method

# generateLicense(attr:)

Generates a license based on the provided ALDLicenseAttribute and add it to the session. Multiple licenses can be generated in this session by callling this function multiple times, they get added to the session response.

``` source
func generateLicense(attr: ALDLicenseAttribute) throws
```

## Parameters 

`attr`  

And ALDLicenseAttribute describing the terms of the license and the key objects

## Mentioned in 

Licensing alternative distribution apps

