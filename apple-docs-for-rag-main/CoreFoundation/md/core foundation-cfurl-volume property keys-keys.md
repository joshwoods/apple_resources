

- Core Foundation
- CFURL
-  Volume Property Keys 

API Collection

# Volume Property Keys

Keys that apply to volumes.

## Topics

### Constants

let kCFURLVolumeNameKey: CFString!

The name of the volume, returned as a `CFString` object.

let kCFURLVolumeLocalizedNameKey: CFString!

The user-presentable name of the volume, returned as a `CFString` object.

let kCFURLVolumeLocalizedFormatDescriptionKey: CFString!

Key for the volume’s descriptive format name, returned as a `CFString` object.

let kCFURLVolumeTotalCapacityKey: CFString!

Key for the volume’s capacity in bytes, returned as a `CFNumber` object.

let kCFURLVolumeAvailableCapacityKey: CFString!

Key for the volume’s available capacity in bytes, returned as a `CFNumber` object.

let kCFURLVolumeResourceCountKey: CFString!

Key for the total number of resources on the volume, returned as a `CFNumber` object.

let kCFURLVolumeSupportsPersistentIDsKey: CFString!

Key for determining whether the volume supports persistent IDs, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsSymbolicLinksKey: CFString!

Key for determining whether the volume supports symbolic links, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsHardLinksKey: CFString!

Key for determining whether the volume supports hard links, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsJournalingKey: CFString!

Key for determining whether the volume supports journaling, returned as a `CFBoolean` object.

let kCFURLVolumeIsJournalingKey: CFString!

Key for determining whether the volume is currently journaling, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsSparseFilesKey: CFString!

Key for determining whether the volume supports sparse files, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsZeroRunsKey: CFString!

Key for determining whether the volume supports zero runs, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsCaseSensitiveNamesKey: CFString!

Key for determining whether the volume supports case-sensitive names, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsCasePreservedNamesKey: CFString!

Key for determining whether the volume supports case-preserved names, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsRootDirectoryDatesKey: CFString!

Key for determining whether the volume supports reliable storage of times for the root directory, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsVolumeSizesKey: CFString!

Key for determining whether the volume supports returning volume size information, returned as a `CFBoolean` object. If `true`, volume size information is available as values of the kCFURLVolumeTotalCapacityKey and kCFURLVolumeAvailableCapacityKey keys.

let kCFURLVolumeSupportsRenamingKey: CFString!

Key for determining whether the volume can be renamed, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsAdvisoryFileLockingKey: CFString!

Key for determining whether the volume implements whole-file advisory locks in the style of flock, along with the `O_EXLOCK` and `O_SHLOCK` flags of the open function, returned as a `CFBoolean` object.

let kCFURLVolumeSupportsExtendedSecurityKey: CFString!

Key for determining whether the volume supports extended security (access control lists), returned as a `CFBoolean` object.

let kCFURLVolumeIsBrowsableKey: CFString!

Key for determining whether the volume is visible in GUI-based file-browsing environments, such as the Desktop or the Finder application, returned as a `CFBoolean` object.

let kCFURLVolumeMaximumFileSizeKey: CFString!

Key for the largest file size supported by the volume in bytes, returned as a `CFNumber` object, or `NULL` if it cannot be determined.

let kCFURLVolumeIsEjectableKey: CFString!

Key for determining whether the volume is ejectable from the drive mechanism under software control, returned as a `CFBoolean` object.

let kCFURLVolumeIsRemovableKey: CFString!

Key for determining whether the volume is removable from the drive mechanism, returned as a `CFBoolean` object.

let kCFURLVolumeIsInternalKey: CFString!

Key for determining whether the volume is connected to an internal bus, returned as a `CFBoolean` object, or `NULL` if it cannot be determined.

let kCFURLVolumeIsAutomountedKey: CFString!

Key for determining whether the volume is automounted, returned as a `CFBoolean` object.

let kCFURLVolumeIsLocalKey: CFString!

Key for determining whether the volume is stored on a local device, returned as a `CFBoolean` object.

let kCFURLVolumeIsReadOnlyKey: CFString!

Key for determining whether the volume is read-only, returned as a `CFBoolean` object.

let kCFURLVolumeCreationDateKey: CFString!

Key for the volume’s creation date, returned as a `CFDate` object, or `NULL` if it cannot be determined.

let kCFURLVolumeURLForRemountingKey: CFString!

Key for the URL needed to remount the network volume, returned as a `CFURL` object, or `NULL` if a URL is not available.

let kCFURLVolumeUUIDStringKey: CFString!

Key for the volume’s persistent UUID, returned as a `CFString` object, or `NULL` if a persistent UUID is not available.

## See Also

### File System Constants

Common File System Resource Keys

Keys that are applicable to file system URLs.

File Resource Types

Possible values for the kCFURLFileResourceTypeKey key.

File Property Keys

Keys that apply to properties of files.

iCloud Constants

These constants can be used to determining whether a file is stored in the cloud and to obtain information about its status.

CFError userInfo Dictionary Keys

Keys in the userInfo dictionary of a `CFError` object when certain CFURL functions return an error.

