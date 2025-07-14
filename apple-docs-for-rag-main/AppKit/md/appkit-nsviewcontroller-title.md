

- AppKit
- NSViewController
-  title 

Instance Property

# title

The localized title of the receiver’s primary view.

macOS 10.5+

``` source
@MainActor
var title: String? { get set }
```

## Discussion

You can employ the title property as needed for your app’s user interface, such as to enable a user to choose among multiple named views in a menu or other affordance. The NSViewController class does not use this property for its own purposes.

The title property is key-value coding and key-value observing compliant.

## See Also

### View Properties

var view: NSView

The view controller’s primary view.

