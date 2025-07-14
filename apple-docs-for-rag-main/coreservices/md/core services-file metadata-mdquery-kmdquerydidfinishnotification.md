

- Core Services
- File Metadata
- MDQuery
-  kMDQueryDidFinishNotification 

API Collection

# kMDQueryDidFinishNotification

Indicates that a query has finished with the initial result-gathering phase.

## Overview

The query results list is not updated as a result of this notification.

This notification is only sent to the application’s notification center.

## Topics

### Constants

let kMDQueryDidFinishNotification: CFString!

Posted to indicate that the query has finished the initial result-gathering phase.

## See Also

### Notifications

kMDQueryDidUpdateNotification

Indicates that a query’s results list has change during the live-update phase of a query.

kMDQueryProgressNotification

Indicates that a query’s results list has change during the initial result-gathering phase of a query.

