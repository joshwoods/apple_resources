

- CloudKit
- CKRecordZone
-  zoneID 

Instance Property

# zoneID

The unique ID of the zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var zoneID: CKRecordZone.ID { get }
```

## Discussion

The zone ID contains the name of the zone and the name of the user who owns the zone. Use this property to access both of those values.

## See Also

### Getting the Zone Attributes

var capabilities: CKRecordZone.Capabilities

The capabilities that the zone supports.

struct Capabilities

The capabilities that a record zone supports.

