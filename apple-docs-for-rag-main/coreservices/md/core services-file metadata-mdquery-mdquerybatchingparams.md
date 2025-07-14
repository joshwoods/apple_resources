

- Core Services
- File Metadata
- MDQuery
-  MDQueryBatchingParams 

Structure

# MDQueryBatchingParams

Structure containing the progress notification batchingparameters of a MDQuery.

Mac Catalyst 13.0+macOS 10.4+

``` source
struct MDQueryBatchingParams
```

## Overview

The default batching parameters are undefined and subjectto change.

## Topics

### Initializers

init()

init(first_max_num: Int, first_max_ms: Int, progress_max_num: Int, progress_max_ms: Int, update_max_num: Int, update_max_ms: Int)

### Instance Properties

var first_max_ms: Int

The maximum number of milliseconds that can passbefore the first progress notification is sent. This value is advisory,in that the notification will be triggered at some point after `first_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the initial result-gathering phase of a query.

var first_max_num: Int

The maximum number of results that can accumulatebefore the first progress notification is sent. This value is usedonly during the initial result-gathering phase of a query.

var progress_max_ms: Int

The maximum number of milliseconds that can passbefore additional progress notifications are sent. This value isadvisory, in that the notification will be triggered at some pointafter `progress_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the initial result-gathering phase of a query.

var progress_max_num: Int

The maximum number of results that can accumulatebefore additional progress notifications are sent. This value isused only during the initial result-gathering phase of a query.

var update_max_ms: Int

The maximum number of milliseconds that can passbefore an update notification is sent. This value is advisory, inthat the notification will be triggered at some point after `update_max_ms` millisecondshave passed since the query began accumulating results. This valueis used only during the live-update phase of a query.

var update_max_num: Int

The maximum number of results that can accumulatebefore an update notification is sent. This value is used only duringthe live-update phase of a query.

