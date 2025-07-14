

- UIKit
- UIFocusDebugger
-  help() 

Type Method

# help()

Returns information about how to use the commands of the debugger object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class func help() -> any UIFocusDebuggerOutput
```

## Discussion

Call this method from the `lldb` debugger using the following commands:

- Swift
- Objective-C

```
po UIFocusDebugger.help()
```

```
po [UIFocusDebugger help]
```

The method returns information about how to use the other methods of this class to get information.

