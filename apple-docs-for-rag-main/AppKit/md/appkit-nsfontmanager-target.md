

- AppKit
- NSFontManager
-  target 

Instance Property

# target

The object that receives action messages related to the font manager.

macOS 10.5+

``` source
weak var target: AnyObject? { get set }
```

## See Also

### Accessing the Action Property

var action: Selector

The action sent to the first responder when the user selects a new font from the Font panel or chooses a command from the Font menu.

