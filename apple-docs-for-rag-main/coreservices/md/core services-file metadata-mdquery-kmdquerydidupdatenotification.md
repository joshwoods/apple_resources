

- Core Services
- File Metadata
- MDQuery
-  kMDQueryDidUpdateNotification 

API Collection

# kMDQueryDidUpdateNotification

Indicates that a query’s results list has change during the live-update phase of a query.

## Overview

The info dictionary of the notification can contain `kMDQueryUpdateAddedItems`, `kMDQueryUpdateChangedItems`, and `kMDQueryUpdateRemovedItems` keys.

This notification is only sent to the application’s notification center.

## Topics

### Constants

let kMDQueryDidUpdateNotification: CFString!

Notification posted to indicate that a change has occurred to the query’s results list during the live-update phase of a query’s execution.

## See Also

### Notifications

kMDQueryDidFinishNotification

Indicates that a query has finished with the initial result-gathering phase.

kMDQueryProgressNotification

Indicates that a query’s results list has change during the initial result-gathering phase of a query.

