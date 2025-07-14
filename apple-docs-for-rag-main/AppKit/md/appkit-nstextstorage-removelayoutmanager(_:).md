

- AppKit
- NSTextStorage
-  removeLayoutManager(\_:) 

Instance Method

# removeLayoutManager(\_:)

Removes a layout manager from the text storage object’s set of layout managers.

macOS 10.0+

``` source
func removeLayoutManager(_ aLayoutManager: NSLayoutManager)
```

## Parameters 

`aLayoutManager`  

The layout manager to remove.

## See Also

### Accessing the layout managers

var layoutManagers: [NSLayoutManager]

The layout managers for the text storage object.

func addLayoutManager(NSLayoutManager)

Adds a layout manager to the text storage object’s set of layout managers.

