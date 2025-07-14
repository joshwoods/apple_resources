

- UIKit
- UIViewController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Creates a view controller with the nib file in the specified bundle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    nibName nibNameOrNil: String?,
    bundle nibBundleOrNil: Bundle?
)
```

## Parameters 

`nibNameOrNil`  

The name of the nib file to associate with the view controller. The nib file name should not contain any leading path information. If you specify `nil`, the nibName property is set to `nil`.

`nibBundleOrNil`  

The bundle in which to search for the nib file. This method looks for the nib file in the bundle’s language-specific project directories first, followed by the Resources directory.

## Return Value

A newly initialized UIViewController object.

## Discussion

This is the designated initializer for this class. When using a storyboard to define your view controller and its associated views, you never initialize your view controller class directly. Instead, view controllers are instantiated by the storyboard either automatically when a segue is triggered or programmatically when your app calls the instantiateViewController(withIdentifier:) method of a storyboard object. When instantiating a view controller from a storyboard, iOS initializes the new view controller by calling its init(coder:) method instead of this method and sets the nibName property to a nib file stored inside the storyboard.

The nib file you specify is not loaded right away. It is loaded the first time the view controller’s view is accessed. If you want to perform additional initialization after the nib file is loaded, override the viewDidLoad() method and perform your tasks there.

If you specify `nil` for the `nibName` parameter and you do not override the loadView() method, the view controller searches for a nib file as described in the nibName property.

For more information about how a view controller loads its view, see View Controller Programming Guide for iOS.

## See Also

### Related Documentation

func loadView()

Creates the view that the controller manages.

var nibBundle: Bundle?

The view controller’s nib bundle if it exists.

var nibName: String?

The name of the view controller’s nib file, if one was specified.

var storyboard: UIStoryboard?

The storyboard from which the view controller originated.

### Creating a view controller

init?(coder: NSCoder)

Creates a view controller with data in an unarchiver.

