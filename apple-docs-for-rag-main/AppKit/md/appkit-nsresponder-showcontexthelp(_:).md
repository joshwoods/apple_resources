

- AppKit
- NSResponder
-  showContextHelp(\_:) 

Instance Method

# showContextHelp(\_:)

Implemented by subclasses to invoke the help system, displaying information relevant to the receiver and its current state.

macOS

``` source
@MainActor
func showContextHelp(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that invoked this method.

## See Also

### Related Documentation

func helpRequested(NSEvent)

Displays context-sensitive help for the receiver if help has been registered.

