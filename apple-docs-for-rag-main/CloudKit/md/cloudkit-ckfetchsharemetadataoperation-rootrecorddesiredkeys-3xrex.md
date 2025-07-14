

- CloudKit
- CKFetchShareMetadataOperation
-  rootRecordDesiredKeys 

Instance Property

# rootRecordDesiredKeys

The fields to return when fetching the root record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
var rootRecordDesiredKeys: [CKRecord.FieldKey]? { get set }
```

## Discussion

For a shared record hierarchy, and when shouldFetchRootRecord is true, set this property to specify which of the root record’s fields the operation fetches. Use `nil` to fetch the entire record. CloudKit ignores this property for a shared record zone because, unlike a hierarchy, it doesn’t have a nominated root record.

The default value is `nil`.

