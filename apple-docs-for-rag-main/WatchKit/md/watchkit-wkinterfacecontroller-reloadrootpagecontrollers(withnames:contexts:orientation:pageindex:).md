

- WatchKit
- WKInterfaceController
-  reloadRootPageControllers(withNames:contexts:orientation:pageIndex:) 

Type Method

# reloadRootPageControllers(withNames:contexts:orientation:pageIndex:)

Loads the specified interface controllers and rebuilds the app’s page-based interface for the given scrolling orientation.

watchOS 4.0+

``` source
@MainActor
class func reloadRootPageControllers(
    withNames names: [String],
    contexts: [Any]?,
    orientation: WKPageOrientation,
    pageIndex: Int
)
```

## Parameters 

`names`  

An array of NSString objects, each of which contains the identifier of an interface controller in your storyboard file. The order of the identifiers in the array defines the order of the corresponding interface controllers in the page-based interface.

`contexts`  

An array of objects of type `id`. Use this parameter to pass context objects to each of the interface controllers loaded into the page-based interface. The first object in the array is passed to the first interface controller, the second object is passed to the second interface controller, and so on.

`orientation`  

The scrolling orientation for the page-based interface. For a list of valid values, see WKPageOrientation.

`pageIndex`  

The index of the page that the system displays in the page-based interface.

## Mentioned in 

Navigating Between Scenes

## Discussion

Call this method to create or modify your app’s page-based interface:

- **At launch time.** Use this method to customize the set of pages you want displayed, and to set the scrolling orientation.

- **At runtime.** Use this method to change the active set of pages or the orientation, adding or removing pages as needed.

## See Also

### Navigating a page-based interface

enum WKPageOrientation

Scrolling orientations for page-based interfaces.

class func reloadRootControllers(withNamesAndContexts: [(name: String, context: AnyObject)])

Loads the specified interface controllers and rebuilds the app’s page-based interface.

func becomeCurrentPage()

Displays the interface controller in the page-based interface.

