

- Core Services
- File Metadata
- MDItem
-  File System Metadata Attribute Keys 

API Collection

# File System Metadata Attribute Keys

Metadata attribute keys that describe the file system attributes for a file.

## Topics

### Constants

let kMDItemDisplayName: CFString!

The localized version of the file name. A CFString.

let kMDItemFSContentChangeDate: CFString!

The date the file contents last changed. A CFDate.

let kMDItemFSCreationDate: CFString!

The date and time that the file was created. A CFDate.

let kMDItemFSInvisible: CFString!

Indicates whether the file is invisible. A CFBoolean.

let kMDItemFSIsExtensionHidden: CFString!

Indicates whether the file extension of the file is hidden. A CFBoolean.

let kMDItemFSLabel: CFString!

Index of the Finder label of the file. Possible values are 0 through 7. A CFNumber.

let kMDItemFSName: CFString!

The file name of the item. A CFString.

let kMDItemFSNodeCount: CFString!

Number of files in a directory. A CFNumber.

let kMDItemFSOwnerGroupID: CFString!

The group ID of the owner of the file. A CFNumber.

let kMDItemFSOwnerUserID: CFString!

The user ID of the owner of the file. A CFNumber.

let kMDItemFSSize: CFString!

The size, in bytes, of the file on disk. A CFNumber.

let kMDItemPath: CFString!

The complete path to the file. A CFString.

