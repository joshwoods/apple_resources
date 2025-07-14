

- CloudKit
- CKContainer
-  accountStatus(completionHandler:) 

Instance Method

# accountStatus(completionHandler:)

Determines whether the system can access the user’s iCloud account.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func accountStatus(completionHandler: @escaping (CKAccountStatus, (any Error)?) -> Void)
```

``` source
func accountStatus() async throws -> CKAccountStatus
```

## Parameters 

`completionHandler`  

The handler to execute when the call completes.

## Discussion

The closure has no return value and takes the following parameters:

- The status of the user’s iCloud account.

- An error that describes the failure, or `nil` if the system successfully determines the status.

This method determines the status of the user’s iCloud account asynchronously, passing the results to the closure that you provide. Call this method before accessing the private database to determine whether that database is available. While your app is running, use the CKAccountChanged notification to detect account changes, and call this method again to determine the status of the new account.

## See Also

### Determining the User’s iCloud Access Status

enum CKAccountStatus

Constants that indicate the availability of the user’s iCloud account.

