

- AVFoundation
- AVContentKeySession
-  pendingExpiredSessionReports(withAppIdentifier:storageDirectoryAt:) 

Type Method

# pendingExpiredSessionReports(withAppIdentifier:storageDirectoryAt:)

Returns the expired session reports for content key sessions created with the specified app identifier.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func pendingExpiredSessionReports(
    withAppIdentifier appIdentifier: Data,
    storageDirectoryAt storageURL: URL
) -> [Data]
```

## Parameters 

`appIdentifier`  

The opaque identifier for the app.

`storageURL`  

The URL that points to the directory containing expired session reports.

## Return Value

Returns an array of expired session reports.

## Discussion

The system only returns expired session reports. It doesn’t include reports for active sessions.

## See Also

### Handling Expired Session Reports

class func removePendingExpiredSessionReports([Data], withAppIdentifier: Data, storageDirectoryAt: URL)

Removes expired session reports from storage.

