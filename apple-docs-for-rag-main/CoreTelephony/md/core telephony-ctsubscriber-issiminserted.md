

- Core Telephony
- CTSubscriber
-  isSIMInserted 

Instance Property

# isSIMInserted

A Boolean property that indicates whether a SIM is present.

iOS 18.0+iPadOS 18.0+

``` source
var isSIMInserted: Bool { get }
```

## Discussion

This value property is `true` if the system finds a SIM matching the `Info.plist` carrier information (MCC / MNC / GID1 / GID2).

