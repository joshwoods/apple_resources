

- AppKit
- NSViewController
-  loadView() 

Instance Method

# loadView()

Instantiates a view from a nib file and sets the value of the view property.

macOS 10.5+

``` source
@MainActor
func loadView()
```

## Discussion

This method connects an instantiated view from a nib file to the view property of the view controller. This method is called by the system, and is exposed in this class so you can override it to add behavior immediately before or after nib loading.

Do not call this method. If you require this method to be called, access the view property.

Do not invoke this method from other objects unless you take care to avoid redundant invocations. The default implementation of the loadView() method handles redundant invocations correctly, but a view controller subclass might not. To be safe, other objects should instead access a view controller’s view property.

The loadView() method first obtains the values of the view controller’s nibName and nibBundle properties. It then employs the NSNib class to instantiate the specified nib file via the instantiate(withOwner:topLevelObjects:) method, providing the view controller object as the `owner` parameter.

For this method to work correctly, you need to have specified the file’s owner of the nib file, in Interface Builder, to be NSViewController. You also need to have correctly connected the `view` outlet of the file’s owner to the intended view in the nib file. Then, at runtime, the nib loading machinery sets the value of the view controller’s view property to the nib file’s instantiated view.

Prior to OS X v10.10, the loadView() method did not provide well-defined behavior if the nibName property’s value was `nil`. In macOS 10.10 and later, however, you get correct behavior without specifying a nib name as long as the nib file’s name is the same as that of the view controller. For example, if you have a view controller subclass called `MyViewController` and a nib file with the same name, you can employ the convenient initialization pattern `[[MyViewController alloc] init]`.

## See Also

### Related Documentation

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

### Creating A View Controller

init(nibName: NSNib.Name?, bundle: Bundle?)

Returns a view controller object initialized to the nib file in the specified bundle.

