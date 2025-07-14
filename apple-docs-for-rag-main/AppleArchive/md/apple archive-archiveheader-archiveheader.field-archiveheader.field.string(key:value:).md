

- Apple Archive
- ArchiveHeader
- ArchiveHeader.Field
-  ArchiveHeader.Field.string(key:value:) 

Case

# ArchiveHeader.Field.string(key:value:)

An enumeration that indicates the field is a string.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case string(
    key: ArchiveHeader.FieldKey,
    value: String
)
```

## See Also

### Field Constants

case blob(key: ArchiveHeader.FieldKey, size: UInt64, offset: UInt64)

An enumeration that indicates the field is a data blob.

case flag(key: ArchiveHeader.FieldKey)

An enumeration that indicates the field is a flag.

case hash(key: ArchiveHeader.FieldKey, hashFunction: ArchiveHash, value: ContiguousArray&lt;UInt8>)

An enumeration that indicates the field is a hash.

case timespec(key: ArchiveHeader.FieldKey, value: timespec)

An enumeration that indicates the field is a time value.

case uint(key: ArchiveHeader.FieldKey, value: UInt64)

An enumeration that indicates the field is an unsigned integer.

