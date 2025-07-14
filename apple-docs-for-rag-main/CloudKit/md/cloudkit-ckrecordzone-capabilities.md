

- CloudKit
- CKRecordZone
-  capabilities 

Instance Property

# capabilities

The capabilities that the zone supports.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var capabilities: CKRecordZone.Capabilities { get }
```

## Discussion

The server determines the capabilities of the zone and sets the value of this property when you save the record zone. Always check this property before performing tasks that require a specific capability.

Default zones don’t support any special capabilities. Custom zones in a private database support the options that CKRecordZone.Capabilities provides.

## See Also

### Getting the Zone Attributes

var zoneID: CKRecordZone.ID

The unique ID of the zone.

struct Capabilities

The capabilities that a record zone supports.

