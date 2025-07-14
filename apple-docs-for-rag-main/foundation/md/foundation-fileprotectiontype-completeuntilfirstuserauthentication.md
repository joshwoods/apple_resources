

- Foundation
- FileProtectionType
-  completeUntilFirstUserAuthentication 

Type Property

# completeUntilFirstUserAuthentication

The file is stored in an encrypted format on disk and cannot be accessed until after the device has booted.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let completeUntilFirstUserAuthentication: FileProtectionType
```

## Discussion

After the user unlocks the device for the first time, your app can access the file and continue to access it even if the user subsequently locks the device.

## See Also

### Working with Protection Levels

static let complete: FileProtectionType

The file is stored in an encrypted format on disk and cannot be read from or written to while the device is locked or booting.

static let completeUnlessOpen: FileProtectionType

The file is stored in an encrypted format on disk after it is closed.

static let none: FileProtectionType

The file has no special protections associated with it.

