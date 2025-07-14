

- App License Delivery SDK
- ALDLicenseAttribute
-  duration 

Instance Property

# duration

The maximum amount of time, in seconds, that iOS considers the license valid.

``` source
var duration: UInt64
```

## Mentioned in 

Licensing alternative distribution apps

Renewing and revoking app licenses

## Discussion

The alternative app marketplace determines a value for this property at its discretion. iOS doesn’t let an app launch if the duration of its license lapses.

A value of `0` indicates that the license doesn’t expire. To revoke a license, see Renewing and revoking app licenses.

For an example that sets this property, see Licensing alternative distribution apps.

