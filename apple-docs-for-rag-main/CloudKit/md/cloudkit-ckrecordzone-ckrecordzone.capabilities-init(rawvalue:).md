

- CloudKit
- CKRecordZone
- CKRecordZone.Capabilities
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a set of capabilities for a record zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init(rawValue: UInt)
```

## Parameters 

`rawValue`  

An integer that represents the combined set of capabilities to create.

## Discussion

Capabilities on record zones that you create locally aren’t valid until you save the record zone. Capabilities on record zones that you fetch from the server are always valid.

