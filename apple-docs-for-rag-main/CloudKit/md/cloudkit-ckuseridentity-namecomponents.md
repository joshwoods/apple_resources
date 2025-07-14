

- CloudKit
- CKUserIdentity
-  nameComponents 

Instance Property

# nameComponents

The user’s name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var nameComponents: PersonNameComponents? { get }
```

## Discussion

You can use this property to construct the user’s name for display. Use the components with an instance of PersonNameComponentsFormatter to create a string representation for the current locale.

## See Also

### Accessing User Information

var userRecordID: CKRecord.ID?

The user record ID for the corresponding user record.

var contactIdentifiers: [String]

Identifiers that match contacts in the local Contacts database.

Deprecated

