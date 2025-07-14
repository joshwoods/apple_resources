

- Core Data
- NSEntityDescription
-  versionHashModifier 

Instance Property

# versionHashModifier

The version hash modifier for the receiver.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var versionHashModifier: String? { get set }
```

## Discussion

This value is included in the version hash for the entity. You use it to mark or denote an entity as being a different “version” than another even if all of the values which affect persistence are equal. (Such a difference is important in cases where, for example, the structure of an entity is unchanged but the format or content of data has changed.)

## See Also

### Managing versioning

var versionHash: Data

The version hash for the receiver.

