

- WatchKit
- WKCrownSequencer
-  delegate 

Instance Property

# delegate

The object you use to monitor changes to the crown state.

watchOS 3.0+

``` source
weak var delegate: (any WKCrownDelegate)? { get set }
```

## Discussion

Assign a delegate object to receive notifications about crown rotation events. For more information about receiving crown-related data, see WKCrownDelegate.

