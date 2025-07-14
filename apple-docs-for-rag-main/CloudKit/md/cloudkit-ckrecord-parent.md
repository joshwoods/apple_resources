

- CloudKit
- CKRecord
-  parent 

Instance Property

# parent

A reference to the record’s parent record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var parent: CKRecord.Reference? { get set }
```

## Discussion

Use parent references to inform CloudKit about the hierarchy of your records. CloudKit shares the hierarchy when a CKShare includes a referenced record. Add relationships between records as you create them, even if you don’t plan to share them. This allows you to manage the sharing of a hierarchy by only modifying the root record’s share reference.

To indicate that a record belongs to its parent, set this property to a reference that points to the parent record. The reference must use the CKRecord.ReferenceAction.none action or CloudKit throws an exception. The parent record must exist on the server when you save the child, or must be part of the same save operation. Otherwise, the operation fails.

## See Also

### Sharing Records

var share: CKRecord.Reference?

A reference to the share object that determines the share status of the record.

class Reference

A relationship between two records in a record zone.

func setParent(CKRecord?)

Creates and sets a reference object for a parent from its record.

func setParent(CKRecord.ID?)

Creates and sets a reference object for a parent from the parent’s record ID.

enum SystemFieldKey

Possible values for types of system field keys on records.

