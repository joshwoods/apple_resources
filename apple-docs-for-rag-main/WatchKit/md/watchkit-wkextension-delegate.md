

- WatchKit
- WKExtension
-  delegate 

Instance Property

# delegate

The delegate of the WatchKit extension object.

watchOS 2.0+

``` source
@MainActor
weak var delegate: (any WKExtensionDelegate)? { get }
```

## Discussion

The delegate object is an object that conforms to the WKExtensionDelegate protocol. You provide the delegate object and use it to manage lifecycle events in your extension. Providing a delegate object is required if your extension supports actionable notifications or Handoff behaviors.

For more information about the methods of the delegate object, see WKExtensionDelegate.

## See Also

### Accessing the extension delegate

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

