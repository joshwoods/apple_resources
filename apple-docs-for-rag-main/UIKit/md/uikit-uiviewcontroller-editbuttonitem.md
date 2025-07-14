

- UIKit
- UIViewController
-  editButtonItem 

Instance Property

# editButtonItem

Returns a bar button item that toggles its title and associated state between Edit and Done.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var editButtonItem: UIBarButtonItem { get }
```

## Discussion

If one of the custom views of the navigationItem property is set to the returned object, the associated navigation bar displays an Edit button if isEditing is false and a Done button if isEditing is true. The default button action invokes the setEditing(_:animated:) method.

## See Also

### Adding editing behaviors to your view controller

var isEditing: Bool

A Boolean value indicating whether the view controller currently allows the user to edit the view contents.

func setEditing(Bool, animated: Bool)

Sets whether the view controller shows an editable view.

