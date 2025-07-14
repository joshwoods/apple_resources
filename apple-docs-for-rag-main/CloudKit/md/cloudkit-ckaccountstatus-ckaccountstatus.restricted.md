

- CloudKit
- CKAccountStatus
-  CKAccountStatus.restricted 

Case

# CKAccountStatus.restricted

The system denies access to the user’s iCloud account.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case restricted
```

## Discussion

Your app can’t access the user’s iCloud account due to restrictions that Parental Controls or Mobile Device Management impose.

## See Also

### Account Statuses

case available

The user’s iCloud account is available.

case couldNotDetermine

CloudKit can’t determine the status of the user’s iCloud account.

case noAccount

The device doesn’t have an iCloud account.

case temporarilyUnavailable

The user’s iCloud account is temporarily unavailable.

