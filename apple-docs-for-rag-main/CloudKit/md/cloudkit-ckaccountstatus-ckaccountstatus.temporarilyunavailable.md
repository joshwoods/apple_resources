

- CloudKit
- CKAccountStatus
-  CKAccountStatus.temporarilyUnavailable 

Case

# CKAccountStatus.temporarilyUnavailable

The user’s iCloud account is temporarily unavailable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case temporarilyUnavailable
```

## Discussion

You receive this account status when the user’s iCloud account is available, but isn’t ready to support CloudKit operations. Don’t delete any cached data and don’t enqueue any CloudKit operations after receipt of this account status. Instead, use the CKAccountChanged notification to listen for when the status changes to CKAccountStatus.available.

## See Also

### Account Statuses

case available

The user’s iCloud account is available.

case couldNotDetermine

CloudKit can’t determine the status of the user’s iCloud account.

case noAccount

The device doesn’t have an iCloud account.

case restricted

The system denies access to the user’s iCloud account.

