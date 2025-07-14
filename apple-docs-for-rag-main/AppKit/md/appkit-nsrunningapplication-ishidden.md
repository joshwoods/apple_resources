

- AppKit
- NSRunningApplication
-  isHidden 

Instance Property

# isHidden

Indicates whether the application is currently hidden.

macOS 10.6+

``` source
var isHidden: Bool { get }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Hiding and unhiding applications

func hide() -> Bool

Attempts to hide or the application.

func unhide() -> Bool

Attempts to unhide or the application.

