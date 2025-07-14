

- Core Data
- NSEntityMappingType
-  NSEntityMappingType.addEntityMappingType 

Case

# NSEntityMappingType.addEntityMappingType

Specifies that this is a new entity in the destination model.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case addEntityMappingType
```

## Discussion

Instances of the entity only exist in the destination.

## See Also

### Constants

case undefinedEntityMappingType

Specifies that the developer handles destination instance creation.

case customEntityMappingType

Specifies a custom mapping.

case removeEntityMappingType

Specifies that this entity is not present in the destination model.

case copyEntityMappingType

Specifies that source instances are migrated as-is.

case transformEntityMappingType

Specifies that entity exists in source and destination and is mapped.

