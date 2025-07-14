

- CloudKit
- CKQuerySubscription
-  init(recordType:predicate:options:) 

Initializer

# init(recordType:predicate:options:)

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOSwatchOS 6.0–6.0DeprecatedSwift 4.2+

``` source
convenience init(
    recordType: CKRecord.RecordType,
    predicate: NSPredicate,
    options querySubscriptionOptions: CKQuerySubscription.Options = [.firesOnRecordCreation, .firesOnRecordUpdate, .firesOnRecordDeletion]
)
```

