

- Core Services
- File Metadata
- MDQuery
- MDQueryBatchingParams
-  update_max_ms 

Instance Property

# update_max_ms

The maximum number of milliseconds that can passbefore an update notification is sent. This value is advisory, inthat the notification will be triggered at some point after `update_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the live-update phase of a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
var update_max_ms: Int
```

