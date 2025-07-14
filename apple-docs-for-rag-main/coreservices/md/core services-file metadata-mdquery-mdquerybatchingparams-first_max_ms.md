

- Core Services
- File Metadata
- MDQuery
- MDQueryBatchingParams
-  first_max_ms 

Instance Property

# first_max_ms

The maximum number of milliseconds that can passbefore the first progress notification is sent. This value is advisory,in that the notification will be triggered at some point after `first_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the initial result-gathering phase of a query.

Mac Catalyst 13.0+macOS 10.4+

``` source
var first_max_ms: Int
```

