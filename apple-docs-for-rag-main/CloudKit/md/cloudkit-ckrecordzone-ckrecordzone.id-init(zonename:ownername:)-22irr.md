

- CloudKit
- CKRecordZone
- CKRecordZone.ID
-  init(zoneName:ownerName:) 

Initializer

# init(zoneName:ownerName:)

Creates a record zone ID with the specified name and owner.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
convenience init(
    zoneName: String = CKRecordZone.ID.defaultZoneName,
    ownerName: String = CKCurrentUserDefaultName
)
```

## Parameters 

`zoneName`  

The name that identifies the record zone. Zone names consist of up to 255 ASCII characters, and don’t start with an underscore. To specify the default zone of the current database, use defaultZoneName. This parameter must not be `nil` or an empty string.

`ownerName`  

The user who creates the record zone. To specify the current user, use CKCurrentUserDefaultName. If you provide `nil` or an empty string for this parameter, the method throws an exception.

## Return Value

A new record zone ID, or `nil` if CloudKit can’t create the record zone ID.

