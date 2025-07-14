

- Foundation
- Archives and Serialization
- NSKeyedArchiver
-  Keyed Archiver Root Object Key 

API Collection

# Keyed Archiver Root Object Key

Keys that the archiver uses in the hierarchy of encoded objects.

## Topics

### Constants

let NSKeyedArchiveRootObjectKey: String

Archives created using the class method archivedData(withRootObject:) use this key for the root object in the hierarchy of encoded objects. The NSKeyedUnarchiver class method unarchiveObject(with:) looks for this root key as well.

## See Also

### Constants

Keyed Archiving Exception Names

Names of exceptions raised by this class if problems occur while creating an archive.

