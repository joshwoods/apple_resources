

- Foundation
- NSDictionary
-  fileSystemNumber() 

Instance Method

# fileSystemNumber()

Returns the filesystem number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fileSystemNumber() -> Int
```

## Return Value

The value associated with the systemNumber file attributes key as an `Int` (`unsigned long` in Objective-C), or `0` if the file attributes dictionary has no entry for the key

## See Also

### Accessing File Attributes

func fileSize() -> UInt64

Returns the file’s size, in bytes.

func fileType() -> String?

Returns the file type.

func fileCreationDate() -> Date?

Returns the file’s creation date.

func fileModificationDate() -> Date?

Returns file’s modification date.

func filePosixPermissions() -> Int

Returns the file’s POSIX permissions.

func fileOwnerAccountID() -> NSNumber?

Returns the file’s owner account ID.

func fileOwnerAccountName() -> String?

Returns the file’s owner account name.

func fileGroupOwnerAccountID() -> NSNumber?

Returns file’s group owner account ID.

func fileGroupOwnerAccountName() -> String?

Returns the file’s group owner account name.

func fileExtensionHidden() -> Bool

Returns a Boolean value indicating whether the file hides its extension.

func fileIsImmutable() -> Bool

Returns a Boolean value indicating whether the file is immutable.

func fileIsAppendOnly() -> Bool

Returns a Boolean value indicating whether the file is append only.

func fileSystemFileNumber() -> Int

Returns the filesystem file number.

func fileHFSTypeCode() -> OSType

Returns file’s HFS type code.

func fileHFSCreatorCode() -> OSType

Returns the file’s HFS creator code.

