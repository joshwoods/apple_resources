

- Foundation
- URLResourceValues
-  volumeIsEjectable 

Instance Property

# volumeIsEjectable

A Boolean value that indicates whether the volume’s media is ejectable from the drive mechanism under software control.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var volumeIsEjectable: Bool? { get }
```

## See Also

### Volume status values

var volumeIsAutomounted: Bool?

A Boolean value that indicates whether the volume is automounted.

var volumeIsBrowsable: Bool?

A Boolean value that indicates whether the volume is visible through the user interface.

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

var volumeTypeName: String?

The volume’s type name, as a string.

var volumeSubtype: Int?

An integer value that indicates the file system subtype.

var volumeMountFromLocation: String?

The file system device location, as a string.

