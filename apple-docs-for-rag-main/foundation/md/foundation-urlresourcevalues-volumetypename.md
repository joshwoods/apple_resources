

- Foundation
- URLResourceValues
-  volumeTypeName 

Instance Property

# volumeTypeName

The volume’s type name, as a string.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
var volumeTypeName: String? { get }
```

## See Also

### Volume status values

var volumeIsAutomounted: Bool?

A Boolean value that indicates whether the volume is automounted.

var volumeIsBrowsable: Bool?

A Boolean value that indicates whether the volume is visible through the user interface.

var volumeIsEjectable: Bool?

A Boolean value that indicates whether the volume’s media is ejectable from the drive mechanism under software control.

var volumeIsEncrypted: Bool?

A Boolean value that indicates whether the volume is encrypted.

var volumeIsInternal: Bool?

A Boolean value that indicates whether the volume’s device is connected to an internal bus, or nil if not available.

var volumeIsJournaling: Bool?

A Boolean value that indicates whether the volume is currently using a journal for speedy recovery after an unplanned restart.

var volumeIsLocal: Bool?

A Boolean value that indicates whether the volume is on a local device.

var volumeIsReadOnly: Bool?

A Boolean value that indicates whether the volume is read-only.

var volumeIsRemovable: Bool?

A Boolean value that indicates whether the volume’s media is removable from the drive mechanism.

var volumeIsRootFileSystem: Bool?

A Boolean value that indicates whether the volume is the root file system.

var volumeSubtype: Int?

An integer value that indicates the file system subtype.

var volumeMountFromLocation: String?

The file system device location, as a string.

