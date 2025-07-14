

- AppKit
- NSSavePanel
-  ok(\_:) 

Instance Method

# ok(\_:)

The action method that the panel calls when the user clicks the OK button.

macOS

``` source
@IBAction @MainActor
func ok(_ sender: Any?)
```

## Parameters 

`sender`  

The NSSavePanel object that contains the OK button.

## Discussion

In macOS 10.15 and later, you cannot call this method programmatically to trigger the OK action. Prior to macOS 10.15, AppKit prevented only sandboxed apps from calling this method.

## See Also

### Handling Actions

func cancel(Any?)

The action method that the panel calls when the user clicks the Cancel button.

