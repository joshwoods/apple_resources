

- UIKit
- UINavigationItem
-  backButtonTitle 

Instance Property

# backButtonTitle

The custom title of the Back button.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var backButtonTitle: String? { get set }
```

## Discussion

Use this property to set the title of the Back button when a view controller’s navigationItem is the backItem of the navigation bar, in other words, when the Back button appears in the navigation bar of the next view controller. For example, a view controller that displays a list of contacts can set backButtonTitle to “Contacts”. When a person taps a contact, the view controller pushes a new view controller onto the navigation stack, which displays the details of the selected contact. This new topmost view controller shows “Contacts” as the Back button title.

Interface Builder shows this behavior when setting the Back button title in a storyboard, as shown in the following screenshot:

When setting backButtonTitle programmatically, set it in the current view controller before pushing a new view controller onto the navigation stack; for instance, in viewDidLoad() or viewWillAppear(_:).

```
override func viewDidLoad() {
    super.viewDidLoad()
    navigationItem.backButtonTitle = "Contacts"
}
```

When backButtonTitle is `nil`, which is the default value, the navigation item uses its title property as the Back button title.

Note

backBarButtonItem takes precedence if you specify both backButtonTitle and backBarButtonItem.

## See Also

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode

The display mode of the Back button.

enum BackButtonDisplayMode

Constants that describe the display modes of the Back button.

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

var backAction: UIAction?

The back action for the navigation bar.

