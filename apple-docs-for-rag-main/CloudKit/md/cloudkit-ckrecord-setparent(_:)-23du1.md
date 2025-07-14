

- CloudKit
- CKRecord
-  setParent(\_:) 

Instance Method

# setParent(\_:)

Creates and sets a reference object for a parent from its record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func setParent(_ parentRecord: CKRecord?)
```

## Parameters 

`parentRecord`  

A record that you want to set as the parent to this record.

## Discussion

This method creates and sets a CKRecord.Reference object that points to the record you provide. The resulting `CKReference` has an action of CKRecord.ReferenceAction.none.

## See Also

### Sharing Records

var parent: CKRecord.Reference?

A reference to the record’s parent record.

var share: CKRecord.Reference?

A reference to the share object that determines the share status of the record.

class Reference

A relationship between two records in a record zone.

func setParent(CKRecord.ID?)

Creates and sets a reference object for a parent from the parent’s record ID.

enum SystemFieldKey

Possible values for types of system field keys on records.

