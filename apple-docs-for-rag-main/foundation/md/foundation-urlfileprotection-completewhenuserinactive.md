

- Foundation
- URLFileProtection
-  completeWhenUserInactive 

Type Property

# completeWhenUserInactive

An option that instructs the system to store the file in an encrypted format on-disk that your app can access only after device unlock and before expiration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let completeWhenUserInactive: URLFileProtection
```

## Discussion

After the first unlock, your app can access the file and continue to access it even if the person using it subsequently locks the device. After access expires, your app can’t access the file until the person using the device unlocks it again.

## See Also

### Protection levels

static let complete: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access for reading or writing to while the device is locked or booting.

static let completeUnlessOpen: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk after it closes.

static let completeUntilFirstUserAuthentication: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access until after the device boots.

static let none: URLFileProtection

An option that indicates the file has no special protections associated with it.

