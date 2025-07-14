

- InputMethodKit
- IMKServer
-  bundle() 

Instance Method

# bundle()

Returns an `NSBundle` object for the input method.

macOS 10.5+

``` source
func bundle() -> Bundle!
```

## Return Value

An `NSBundle` object that is either created from the bundle identifier contained in the server object, or from the main bundle.

