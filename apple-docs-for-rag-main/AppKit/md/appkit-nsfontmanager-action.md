

- AppKit
- NSFontManager
-  action 

Instance Property

# action

The action sent to the first responder when the user selects a new font from the Font panel or chooses a command from the Font menu.

macOS

``` source
var action: Selector { get set }
```

## Discussion

The default action is changeFont:. You should rarely need to change this setting.

## See Also

### Accessing the Action Property

var target: AnyObject?

The object that receives action messages related to the font manager.

