

- Swift
- UnsafeCurrentTask
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that indicates whether the current task was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

After the value of this property becomes `true`, it remains `true` indefinitely. There is no way to uncancel a task.

See Also

`checkCancellation()`

