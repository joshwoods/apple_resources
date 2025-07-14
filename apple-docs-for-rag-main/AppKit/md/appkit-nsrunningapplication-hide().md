

- AppKit
- NSRunningApplication
-  hide() 

Instance Method

# hide()

Attempts to hide or the application.

macOS 10.6+

``` source
func hide() -> Bool
```

## Return Value

true if the application was successfully hidden, otherwise false.

## Mentioned in 

Passing control from one app to another with cooperative activation

## Discussion

The property of this value will be false if the application has already quit, or if of a type that is unable to be hidden.

## See Also

### Hiding and unhiding applications

func unhide() -> Bool

Attempts to unhide or the application.

var isHidden: Bool

Indicates whether the application is currently hidden.

