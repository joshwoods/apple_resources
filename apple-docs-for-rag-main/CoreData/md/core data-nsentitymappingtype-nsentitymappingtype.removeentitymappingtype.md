

- Core Data
- NSEntityMappingType
-  NSEntityMappingType.removeEntityMappingType 

Case

# NSEntityMappingType.removeEntityMappingType

Specifies that this entity is not present in the destination model.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case removeEntityMappingType
```

## Discussion

Instances of the entity only exist in the source—source instances are not mapped to destination.

## See Also

### Constants

case undefinedEntityMappingType

Specifies that the developer handles destination instance creation.

case customEntityMappingType

Specifies a custom mapping.

case addEntityMappingType

Specifies that this is a new entity in the destination model.

case copyEntityMappingType

Specifies that source instances are migrated as-is.

case transformEntityMappingType

Specifies that entity exists in source and destination and is mapped.

