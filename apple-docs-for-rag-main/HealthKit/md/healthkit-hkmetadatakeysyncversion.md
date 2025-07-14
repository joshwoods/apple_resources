

- HealthKit
-  HKMetadataKeySyncVersion 

Global Variable

# HKMetadataKeySyncVersion

The version number for a piece of data, used when updating or syncing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
let HKMetadataKeySyncVersion: String
```

## Discussion

This key takes an NSNumber as its value. When you save an object to the HealthKit store, the new object replaces any matching objects (existing objects with a matching HKMetadataKeySyncIdentifier value) with a lower sync version.

For more information, see HKMetadataKeySyncIdentifier.

## See Also

### Sync Keys

let HKMetadataKeySyncIdentifier: String

A unique string that identifies a piece of data so it can be updated and synced.

