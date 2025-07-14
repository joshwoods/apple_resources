

- UIKit
- UIViewController
-  isEditing 

Instance Property

# isEditing

A Boolean value indicating whether the view controller currently allows the user to edit the view contents.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var isEditing: Bool { get set }
```

## Discussion

If true, the view controller currently allows editing; otherwise, false.

If the view is editable and the associated navigation controller contains an edit-done button, then a Done button is displayed; otherwise, an Edit button is displayed. Clicking either button toggles the state of this property. Add an edit-done button by setting the custom left or right view of the navigation item to the value returned by the editButtonItem method. Set the isEditing property to the initial state of your view. Use the setEditing(_:animated:) method as an action method to animate the transition of this state if the view is already displayed.

## See Also

### Adding editing behaviors to your view controller

func setEditing(Bool, animated: Bool)

Sets whether the view controller shows an editable view.

var editButtonItem: UIBarButtonItem

Returns a bar button item that toggles its title and associated state between Edit and Done.

