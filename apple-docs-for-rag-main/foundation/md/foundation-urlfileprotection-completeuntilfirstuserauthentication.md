

- Foundation
- URLFileProtection
-  completeUntilFirstUserAuthentication 

Type Property

# completeUntilFirstUserAuthentication

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access until after the device boots.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let completeUntilFirstUserAuthentication: URLFileProtection
```

## Discussion

After the user unlocks the device for the first time, your app can access the file and continue to access it even if the user subsequently locks the device.

## See Also

### Protection levels

static let complete: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access for reading or writing to while the device is locked or booting.

static let completeUnlessOpen: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk after it closes.

static let completeWhenUserInactive: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can access only after device unlock and before expiration.

static let none: URLFileProtection

An option that indicates the file has no special protections associated with it.

