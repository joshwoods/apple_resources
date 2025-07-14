

- Apple Archive
- ArchiveHeader
-  ArchiveHeader.FieldKey 

Structure

# ArchiveHeader.FieldKey

A type that’s an alias for the field key structure.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct FieldKey
```

## Overview

Apple Archive supports the following predefined keys:

ACL  
An ArchiveHeader.Field.blob(key:size:offset:) enumeration that describes the access control list for directories and regular files only. For more information, see AAEntryACLBlob.

BTM  
An ArchiveHeader.Field.timespec(key:value:) enumeration that describes the backup time.

CKS  
An ArchiveHeader.Field.hash(key:hashFunction:value:) enumeration that describes the checksum of the entry data’s 32-bit cyclic redundancy check for regular files only.

CLC  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the clone-cluster identity for regular files only.

CTM  
An ArchiveHeader.Field.timespec(key:value:) enumeration that describes the creation time.

DAT  
An ArchiveHeader.Field.blob(key:size:offset:) enumeration that describes the entry data for regular files only.

DUZ  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the disk usage.

FLG  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the flags (`st.st_flags`).

GID  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the group identity (`st.st_gid`).

HLC  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the hard-link cluster identity for regular files only.

IDX  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the offset of the entry in the reference archive.

IDZ  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the size of the entry in the reference archive.

INO  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the inode number (`st.st_ino`).

LNK  
An ArchiveHeader.Field.string(key:value:) enumeration that describes the symbolic link path for symbolic links only.

MOD  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the access modes (that is, the low 12 bits of `st.st_mode`).

MTM  
An ArchiveHeader.Field.timespec(key:value:) enumeration that describes the modification time.

PAT  
An ArchiveHeader.Field.string(key:value:) enumeration that describes the entry path.

SH1  
An ArchiveHeader.Field.hash(key:hashFunction:value:) enumeration that describes the entry-data SHA1 hash for regular files only.

SH2  
An ArchiveHeader.Field.hash(key:hashFunction:value:) enumeration that describes the entry-data SHA2-256 hash for regular files only.

SH3  
An ArchiveHeader.Field.hash(key:hashFunction:value:) enumeration that describes the entry-data SHA2-384 hash for regular files only.

SH5  
An ArchiveHeader.Field.hash(key:hashFunction:value:) enumeration that describes the entry-data SHA2-512 hash for regular files only.

SIZ  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the uncompressed data size for regular files only.

SLC  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the identical data-cluster identity for regular files only.

TYP  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the entry type (from the high bits of `st.st_mode`, one of `AA_ENTRY_TYPE_*`).

UID  
An ArchiveHeader.Field.uint(key:value:) enumeration that describes the user identity (`st.st_uid`).

XAT  
An ArchiveHeader.Field.blob(key:size:offset:) enumeration that describes the entry’s extended attributes. For more information, see AAEntryXATBlob.

## Topics

### Field Key Creation

init(String)

Creates a new field key from the key you specify.

### Instance Properties

var description: String

A textual representation of this instance.

### Equatable Requirements

static func == (ArchiveHeader.FieldKey, ArchiveHeader.FieldKey) -> Bool

Equatable protocol

### Hash Values

func hash(into: inout Hasher)

Hashable protocol

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Manipulating Fields

func field(forKey: ArchiveHeader.FieldKey) -> ArchiveHeader.Field?

Returns the field for a specified key.

enum Field

An enumeration that describes the type, key, and value of a header field.

var fieldType: ArchiveHeader._FieldTypes

The field types of the archive header.

struct FieldType

Constants that specify the field type of an archive header.

var fieldKey: ArchiveHeader._FieldKeys

The field keys of the archive header.

class FieldKeySet

An object that represents a field key set.

