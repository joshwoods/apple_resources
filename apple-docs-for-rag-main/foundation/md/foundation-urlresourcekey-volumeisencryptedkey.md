

- Foundation
- URLResourceKey
-  volumeIsEncryptedKey 

Type Property

# volumeIsEncryptedKey

A key for determining whether the volume is encrypted.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let volumeIsEncryptedKey: URLResourceKey
```

## Discussion

The corresponding value is a Boolean `NSNumber` object.

## See Also

### Volume status keys

static let volumeIsAutomountedKey: URLResourceKey

A key for determining whether the volume is automounted.

static let volumeIsBrowsableKey: URLResourceKey

A key for determining whether the volume is visible in GUI-based file-browsing environments, such as the Desktop or the Finder app.

static let volumeIsEjectableKey: URLResourceKey

A key for determining whether the volume is ejectable from the drive mechanism under software control.

static let volumeIsInternalKey: URLResourceKey

A key for determining whether the volume is connected to an internal bus.

static let volumeIsJournalingKey: URLResourceKey

A key for determining whether the volume is currently journaling.

static let volumeIsLocalKey: URLResourceKey

A key for determining whether the volume is on a local device.

static let volumeIsReadOnlyKey: URLResourceKey

A key for determining whether the volume is read-only.

static let volumeIsRemovableKey: URLResourceKey

A key for determining whether the volume is removable from the drive mechanism.

static let volumeIsRootFileSystemKey: URLResourceKey

A key for determining whether the volume is the root file system.

static let volumeSupportsFileProtectionKey: URLResourceKey

A Boolean value that indicates the volume supports data protection for files.

static let volumeTypeNameKey: URLResourceKey

The key for the name of the file system type.

static let volumeSubtypeKey: URLResourceKey

The key for the file system subtype value.

static let volumeMountFromLocationKey: URLResourceKey

The key for the volume mounted-from location.

