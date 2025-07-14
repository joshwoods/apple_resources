

- WatchKit
- WKInterfaceController
-  crownSequencer 

Instance Property

# crownSequencer

The object to use when directly tracking crown events.

watchOS 2.0+

``` source
@MainActor
var crownSequencer: WKCrownSequencer { get }
```

## Discussion

Use the object in this property to monitor crown-related events yourself. You can use this object in an interface that also includes a WKInterfacePicker, but only one of those objects can receive crown events at any given time. For information about how to configure a crown sequencer object, see WKCrownSequencer.

