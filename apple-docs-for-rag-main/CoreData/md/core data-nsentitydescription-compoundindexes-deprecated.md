

- Core Data
- NSEntityDescription
-  compoundIndexes Deprecated

Instance Property

# compoundIndexes

The compound indexes for the entity as an array of arrays.

iOS 3.0–11.0DeprecatediPadOS 3.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
var compoundIndexes: [[Any]] { get set }
```

Deprecated

Use NSEntityDescription.indexes instead

## Discussion

The arrays contained in the returned array contain instances of `NSAttributeDescription`, `NSRelationshipDescription` that represent properties of the entity, or of `NSString` that match the name of attributes or relationships of the entity.

Compound indexes are only used by stores that natively support compound indices—setting them is only advisory. Indexes apply to the entire inheritance hierarchy.

## See Also

### Configuring indexes and constraints

var indexes: [NSFetchIndexDescription]

An array of fetch index descriptions for the entity.

var uniquenessConstraints: [[Any]]

An array of arrays that contains one or more attributes with a value that must be unique over the instances of that entity.

