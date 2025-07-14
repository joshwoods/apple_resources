

- Core Data
- NSAttributeDescription
-  versionHash 

Instance Property

# versionHash

The version hash for the attribute.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var versionHash: Data { get }
```

## Discussion

The version hash is used to uniquely identify an attribute based on its configuration. This value includes the versionHash information from NSPropertyDescription and the attribute type.

## See Also

### Related Documentation

var versionHash: Data

The version hash for the receiver.

