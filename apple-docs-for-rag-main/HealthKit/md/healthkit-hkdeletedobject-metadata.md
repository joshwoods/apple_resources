

- HealthKit
- HKDeletedObject
-  metadata 

Instance Property

# metadata

The metadata associated with the deleted object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
var metadata: [String : Any]? { get }
```

## Discussion

The system only copies the HKMetadataKeySyncIdentifier and HKMetadataKeySyncVersion keys from the original object. All other metadata is lost.

For more information about the metadata’s format and content, see the HKObject class’s metadata property.

## See Also

### Identifying Deleted Objects

var uuid: UUID

The universally unique identifier (UUID) for the HealthKit object that was deleted from the store.

