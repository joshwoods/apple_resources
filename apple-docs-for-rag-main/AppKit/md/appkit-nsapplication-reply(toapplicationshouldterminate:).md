

- AppKit
- NSApplication
-  reply(toApplicationShouldTerminate:) 

Instance Method

# reply(toApplicationShouldTerminate:)

Responds to `NSTerminateLater` once the app knows whether it can terminate.

macOS

``` source
@MainActor
func reply(toApplicationShouldTerminate shouldTerminate: Bool)
```

## Parameters 

`shouldTerminate`  

Specify true if you want the app to terminate; otherwise, specify false.

## Discussion

If your app delegate returns `NSTerminateLater` from its applicationShouldTerminate(_:) method, your code must subsequently call this method to let the `NSApplication` object know whether it can actually terminate itself.

## See Also

### Terminating the App

func terminate(Any?)

Terminates the receiver.

