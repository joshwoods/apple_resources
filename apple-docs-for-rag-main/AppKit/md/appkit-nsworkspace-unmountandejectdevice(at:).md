

- AppKit
- NSWorkspace
-  unmountAndEjectDevice(at:) 

Instance Method

# unmountAndEjectDevice(at:)

Attempts to eject the volume mounted at the given path.

macOS 10.6+

``` source
func unmountAndEjectDevice(at url: URL) throws
```

## Parameters 

`url`  

The URL of the volume to eject.

## Discussion

You can safely call this method from any thread of your app.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Unmounting a Device

func unmountAndEjectDevice(atPath: String) -> Bool

Unmounts and ejects the device at the specified path.

