

- Apple Archive
- ArchiveHeader
- ArchiveHeader.Field
-  ArchiveHeader.Field.flag(key:) 

Case

# ArchiveHeader.Field.flag(key:)

An enumeration that indicates the field is a flag.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case flag(key: ArchiveHeader.FieldKey)
```

## See Also

### Field Constants

case blob(key: ArchiveHeader.FieldKey, size: UInt64, offset: UInt64)

An enumeration that indicates the field is a data blob.

case hash(key: ArchiveHeader.FieldKey, hashFunction: ArchiveHash, value: ContiguousArray&lt;UInt8>)

An enumeration that indicates the field is a hash.

case string(key: ArchiveHeader.FieldKey, value: String)

An enumeration that indicates the field is a string.

case timespec(key: ArchiveHeader.FieldKey, value: timespec)

An enumeration that indicates the field is a time value.

case uint(key: ArchiveHeader.FieldKey, value: UInt64)

An enumeration that indicates the field is an unsigned integer.

