

- Foundation
- URLFileProtection
-  completeUnlessOpen 

Type Property

# completeUnlessOpen

An option that instructs the system to store the file in an encrypted format on-disk after it closes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let completeUnlessOpen: URLFileProtection
```

## Discussion

Files with this type of protection can be created while the device is locked, but once closed, cannot be opened again until the device is unlocked. If the file is opened when unlocked, you may continue to access the file normally, even if the user locks the device. There is a small performance penalty when the file is created and opened, though not when being written to or read from. This can be mitigated by changing the file protection to complete when the device is unlocked.

## See Also

### Protection levels

static let complete: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access for reading or writing to while the device is locked or booting.

static let completeUntilFirstUserAuthentication: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can’t access until after the device boots.

static let completeWhenUserInactive: URLFileProtection

An option that instructs the system to store the file in an encrypted format on-disk that your app can access only after device unlock and before expiration.

static let none: URLFileProtection

An option that indicates the file has no special protections associated with it.

