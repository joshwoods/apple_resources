

- Foundation
- URLFileProtection
-  complete 

Type Property

# complete

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access for reading or writing to while the device is locked or booting.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let complete: URLFileProtection
```

## See Also

### Protection levels

static let completeUnlessOpen: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk after it closes.

static let completeUntilFirstUserAuthentication: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access until after the device boots.

static let completeWhenUserInactive: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can access only after device unlock and before expiration.

static let none: URLFileProtection

An option that indicates the file has no special protections associated with it.

