

- CloudKit
- CKSyncEngineZoneDeletionReason
-  CKSyncEngineZoneDeletionReason.purged 

Case

# CKSyncEngineZoneDeletionReason.purged

The owner of the iCloud account purged your app’s data using the Settings app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case purged
```

## Discussion

Important

Upon receipt of deletions with this reason, you must delete any locally cached data and not resend it to iCloud.

## See Also

### Deletion reasons

case deleted

Your app deleted the record zone.

case encryptedDataReset

The owner of the iCloud account reset their encrypted data.

