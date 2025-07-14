

- Metal
- MTLArgument
-  threadgroupMemoryAlignment Deprecated

Instance Property

# threadgroupMemoryAlignment

The required byte alignment in memory for the threadgroup data.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var threadgroupMemoryAlignment: Int { get }
```

## Discussion

If the argument is not a threadgroup, querying this property is a fatal error. The Metal device determines this value.

## See Also

### Describing a Threadgroup Memory Argument

var threadgroupMemoryDataSize: Int

The size, in bytes, of the threadgroup data.

Deprecated

