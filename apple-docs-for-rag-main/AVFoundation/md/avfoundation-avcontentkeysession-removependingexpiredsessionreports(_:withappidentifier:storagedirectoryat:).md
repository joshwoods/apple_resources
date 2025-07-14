

- AVFoundation
- AVContentKeySession
-  removePendingExpiredSessionReports(\_:withAppIdentifier:storageDirectoryAt:) 

Type Method

# removePendingExpiredSessionReports(\_:withAppIdentifier:storageDirectoryAt:)

Removes expired session reports from storage.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func removePendingExpiredSessionReports(
    _ expiredSessionReports: [Data],
    withAppIdentifier appIdentifier: Data,
    storageDirectoryAt storageURL: URL
)
```

## Parameters 

`expiredSessionReports`  

An array of expired session reports to delete.

`appIdentifier`  

The opaque identifier for the app.

`storageURL`  

The URL that points to the directory containing expired session reports.

## See Also

### Handling Expired Session Reports

class func pendingExpiredSessionReports(withAppIdentifier: Data, storageDirectoryAt: URL) -> [Data]

Returns the expired session reports for content key sessions created with the specified app identifier.

