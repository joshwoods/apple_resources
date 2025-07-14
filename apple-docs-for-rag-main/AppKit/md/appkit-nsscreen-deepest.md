

- AppKit
- NSScreen
-  deepest 

Type Property

# deepest

Returns a screen object representing the screen that can best represent color.

macOS

``` source
class var deepest: NSScreen? { get }
```

## Return Value

The screen with the highest bit depth.

## Discussion

This method always returns an object, even if there is only one screen and it is not a color screen.

## See Also

### Getting Screen Objects

class var main: NSScreen?

Returns the screen object containing the window with the keyboard focus.

class var screens: [NSScreen]

Returns an array of screen objects representing all of the screens available on the system.

