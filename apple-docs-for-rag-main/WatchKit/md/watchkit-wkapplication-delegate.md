

- WatchKit
- WKApplication
-  delegate 

Instance Property

# delegate

The delegate of the WatchKit app object.

watchOS 7.0+

``` source
@MainActor
weak var delegate: (any WKApplicationDelegate)? { get }
```

## Discussion

The delegate object is an object that conforms to the WKApplicationDelegate protocol. You provide the delegate object and use it to manage lifecycle events in your extension. Providing a delegate object is required if your extension supports actionable notifications or Handoff behaviors.

For more information about the methods of the delegate object, see WKApplicationDelegate.

## See Also

### Accessing the app delegate

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

