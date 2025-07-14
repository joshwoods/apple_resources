

- Scripting Bridge
- SBApplication
-  delegate 

Instance Property

# delegate

The error-handling delegate of the receiver.

Mac Catalyst 13.0+macOS 10.5+

``` source
var delegate: (any SBApplicationDelegate)? { get set }
```

## Discussion

The delegate should implement the eventDidFail(_:withError:) method of the SBApplicationDelegate informal protocol.

