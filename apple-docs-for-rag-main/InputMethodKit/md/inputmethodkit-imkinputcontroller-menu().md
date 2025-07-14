

- InputMethodKit
- IMKInputController
-  menu() 

Instance Method

# menu()

Returns a menu of commands that are specific to an input method.

macOS 10.5+

``` source
func menu() -> NSMenu!
```

## Return Value

The menu object.

## Discussion

This method is called whenever the menu needs to be drawn so that an input method can update the menu to reflect the current state.

## See Also

### Working with Custom Commands

func doCommand(by: Selector!, command: [AnyHashable : Any]!)

Passes commands that are not generated as part of the text input process.

