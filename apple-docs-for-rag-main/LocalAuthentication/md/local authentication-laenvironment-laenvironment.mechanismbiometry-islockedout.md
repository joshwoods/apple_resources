

- Local Authentication
- LAEnvironment
- LAEnvironment.MechanismBiometry
-  isLockedOut 

Instance Property

# isLockedOut

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
var isLockedOut: Bool { get }
```

## Discussion

```
        locked out after 5 failed match attempts in row. To recover from bio lockout, users need to enter their passcode
        (e.g. during device ulock).
```

