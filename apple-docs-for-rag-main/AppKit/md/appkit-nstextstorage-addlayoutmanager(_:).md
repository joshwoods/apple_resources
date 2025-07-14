

- AppKit
- NSTextStorage
-  addLayoutManager(\_:) 

Instance Method

# addLayoutManager(\_:)

Adds a layout manager to the text storage object’s set of layout managers.

macOS 10.0+

``` source
func addLayoutManager(_ aLayoutManager: NSLayoutManager)
```

## Parameters 

`aLayoutManager`  

The layout manager to add.

## See Also

### Accessing the layout managers

var layoutManagers: [NSLayoutManager]

The layout managers for the text storage object.

func removeLayoutManager(NSLayoutManager)

Removes a layout manager from the text storage object’s set of layout managers.

