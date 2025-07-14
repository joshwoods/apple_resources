

- Core Data
- NSMappingModel
-  entityMappings 

Instance Property

# entityMappings

The entity mappings for the mapping model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entityMappings: [NSEntityMapping]! { get set }
```

## Discussion

The order of the mappings in the array determines the order in which they will be processed during migration.

## See Also

### Managing Entity Mappings

var entityMappingsByName: [String : NSEntityMapping]

The entity mappings for the mapping model, keyed by name.

