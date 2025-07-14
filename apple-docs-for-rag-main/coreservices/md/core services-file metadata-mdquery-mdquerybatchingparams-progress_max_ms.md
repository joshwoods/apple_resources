

- Core Services
- File Metadata
- MDQuery
- MDQueryBatchingParams
-  progress_max_ms 

Instance Property

# progress_max_ms

The maximum number of milliseconds that can passbefore additional progress notifications are sent. This value isadvisory, in that the notification will be triggered at some pointafter `progress_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the initial result-gathering phase of a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
var progress_max_ms: Int
```

