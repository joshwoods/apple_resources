

- WatchKit
- WKInterfaceController
-  becomeCurrentPage() 

Instance Method

# becomeCurrentPage()

Displays the interface controller in the page-based interface.

watchOS 2.0+

``` source
@MainActor
func becomeCurrentPage()
```

## Mentioned in 

Navigating Between Scenes

## Discussion

Use this method to make the current interface controller become the current page of a page-based interface. The current interface controller must be installed in the page-based interface. After calling this method, WatchKit animates the interface controller into view.

Always call this method from your WatchKit extension’s main thread.

## See Also

### Navigating a page-based interface

class func reloadRootPageControllers(withNames: [String], contexts: [Any]?, orientation: WKPageOrientation, pageIndex: Int)

Loads the specified interface controllers and rebuilds the app’s page-based interface for the given scrolling orientation.

enum WKPageOrientation

Scrolling orientations for page-based interfaces.

class func reloadRootControllers(withNamesAndContexts: [(name: String, context: AnyObject)])

Loads the specified interface controllers and rebuilds the app’s page-based interface.

