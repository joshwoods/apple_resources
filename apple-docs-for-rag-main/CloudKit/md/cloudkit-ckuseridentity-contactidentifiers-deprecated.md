

- CloudKit
- CKUserIdentity
-  contactIdentifiers Deprecated

Instance Property

# contactIdentifiers

Identifiers that match contacts in the local Contacts database.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13–15.0DeprecatedtvOS 11.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 4.0–11.0Deprecated

``` source
var contactIdentifiers: [String] { get }
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Discussion

Identities that CloudKit discovers using CKDiscoverAllUserIdentitiesOperation correspond to entries in the local Contacts database, matching the identifier on CNContact. Use these identifiers with the Contacts database to get additional information about the contacts. Multiple identifiers can exist for a single discovered user because multiple contacts can contain the same email addresses or phone numbers.

To transform these identifiers into an array of unified contact identifiers, create a predicate by calling the predicateForContacts(withIdentifiers:) method, and then pass that predicate to the unifiedContacts(matching:keysToFetch:) method.

## See Also

### Accessing User Information

var userRecordID: CKRecord.ID?

The user record ID for the corresponding user record.

var nameComponents: PersonNameComponents?

The user’s name.

