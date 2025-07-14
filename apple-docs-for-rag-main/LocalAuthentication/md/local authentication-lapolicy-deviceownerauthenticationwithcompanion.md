

- Local Authentication
- LAPolicy
-  deviceOwnerAuthenticationWithCompanion 

Type Property

# deviceOwnerAuthenticationWithCompanion

Device owner will be authenticated by a companion device e.g. Watch, Mac, etc.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
static var deviceOwnerAuthenticationWithCompanion: LAPolicy { get }
```

## Discussion

Companion authentication is required. If no nearby paired companion device can be found, LAErrorCompanionNotAvailable is returned.

```
        Users should follow instructions on the companion device to authenticate.
```

