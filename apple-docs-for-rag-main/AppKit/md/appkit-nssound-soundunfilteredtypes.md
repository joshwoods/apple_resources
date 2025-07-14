

- AppKit
- NSSound
-  soundUnfilteredTypes 

Type Property

# soundUnfilteredTypes

Provides the file types the `NSSound` class understands.

macOS 10.5+

``` source
class var soundUnfilteredTypes: [String] { get }
```

## Return Value

Array of UTIs identifying the file types the `NSSound` class understands.

## See Also

### Getting Sound Information

init?(named: NSSound.Name)

Returns the `NSSound` instance associated with a given name.

var duration: TimeInterval

The duration of the sound, in seconds.

