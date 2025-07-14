

- Foundation
-  NSUbiquitousKeyValueStoreInitialSyncChange 

Global Variable

# NSUbiquitousKeyValueStoreInitialSyncChange

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSUbiquitousKeyValueStoreInitialSyncChange: Int { get }
```

## Discussion

Your attempt to write to key-value storage was discarded because an initial download from iCloud has not yet happened. That is, before you can first write key-value data, the system must ensure that your app’s local, on-disk cache matches the truth in iCloud.

Initial downloads happen the first time a device is connected to an iCloud account, and when a user switches their primary iCloud account.

## See Also

### Constants

var NSUbiquitousKeyValueStoreServerChange: Int

var NSUbiquitousKeyValueStoreQuotaViolationChange: Int

var NSUbiquitousKeyValueStoreAccountChange: Int

