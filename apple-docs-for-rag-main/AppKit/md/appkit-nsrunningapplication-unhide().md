

- AppKit
- NSRunningApplication
-  unhide() 

Instance Method

# unhide()

Attempts to unhide or the application.

macOS 10.6+

``` source
func unhide() -> Bool
```

## Return Value

true if the application was successfully shown, otherwise false.

## Discussion

The property of this value will be false if the application has already quit, or if of a type that is unable to be hidden.

## See Also

### Hiding and unhiding applications

func hide() -> Bool

Attempts to hide or the application.

var isHidden: Bool

Indicates whether the application is currently hidden.

