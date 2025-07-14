

- Foundation
- FileProtectionType
-  none 

Type Property

# none

The file has no special protections associated with it.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let none: FileProtectionType
```

## Discussion

A file with this type of protection can be read from or written to at any time.

## See Also

### Working with Protection Levels

static let complete: FileProtectionType

The file is stored in an encrypted format on disk and cannot be read from or written to while the device is locked or booting.

static let completeUnlessOpen: FileProtectionType

The file is stored in an encrypted format on disk after it is closed.

static let completeUntilFirstUserAuthentication: FileProtectionType

The file is stored in an encrypted format on disk and cannot be accessed until after the device has booted.

