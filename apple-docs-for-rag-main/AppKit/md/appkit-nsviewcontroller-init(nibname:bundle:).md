

- AppKit
- NSViewController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Returns a view controller object initialized to the nib file in the specified bundle.

macOS 10.5+

``` source
@MainActor
init(
    nibName nibNameOrNil: NSNib.Name?,
    bundle nibBundleOrNil: Bundle?
)
```

## Parameters 

`nibNameOrNil`  

The name of the nib file, without any leading path information.

`nibBundleOrNil`  

The bundle in which to search for the nib file. If you specify `nil`, this method looks for the nib file in the main bundle.

## Return Value

The initialized NSViewController object.

## Discussion

The NSViewController object looks for the nib file in the bundle’s language-specific project directories first, followed by the Resources directory.

The specified nib file should typically have the class of the file’s owner set to NSViewController, or a custom subclass, with the `view` outlet connected to a view.

If you pass in `nil` for `nibNameOrNil`, nibName returns `nil` and loadView() throws an exception; in this case you must set view before view is invoked, or override loadView().

## See Also

### Creating A View Controller

func loadView()

Instantiates a view from a nib file and sets the value of the view property.

