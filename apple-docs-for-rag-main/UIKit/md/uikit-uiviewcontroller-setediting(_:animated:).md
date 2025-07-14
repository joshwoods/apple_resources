

- UIKit
- UIViewController
-  setEditing(\_:animated:) 

Instance Method

# setEditing(\_:animated:)

Sets whether the view controller shows an editable view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func setEditing(
    _ editing: Bool,
    animated: Bool
)
```

## Parameters 

`editing`  

If true, the view controller should display an editable view; otherwise, false.

If true and one of the custom views of the navigationItem property is set to the value returned by the editButtonItem method, the associated navigation controller displays a Done button; otherwise, an Edit button.

`animated`  

If true, animates the transition; otherwise, does not.

## Discussion

Subclasses that use an edit-done button must override this method to change their view to an editable state if isEditing is true and a non-editable state if it is false. This method should invoke super’s implementation before updating its view.

## See Also

### Adding editing behaviors to your view controller

var isEditing: Bool

A Boolean value indicating whether the view controller currently allows the user to edit the view contents.

var editButtonItem: UIBarButtonItem

Returns a bar button item that toggles its title and associated state between Edit and Done.

