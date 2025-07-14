

- CloudKit
- CKFetchRecordZonesOperation
-  init(recordZoneIDs:) 

Initializer

# init(recordZoneIDs:)

Creates an operation for fetching the specified record zones.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init(recordZoneIDs zoneIDs: [CKRecordZone.ID])
```

## Parameters 

`zoneIDs`  

An array ofCKRecordZone.ID objects that represents the zones you want to retrieve. If you provide an empty array, you must set the recordZoneIDs property before you execute the operation.

## Discussion

After creating the operation, assign a value to the fetchRecordZonesCompletionBlock property so you can process the results.

## See Also

### Initializing the Zone Fetch Operation

init()

Creates an empty fetch zones operation.

