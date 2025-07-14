

- Shared With You
- SWCollaborationView
-  dismissPopover(\_:) 

Instance Method

# dismissPopover(\_:)

Dismisses the popover.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
func dismissPopover(_ completion: (() -> Void)? = nil)
```

``` source
@MainActor
func dismissPopover() async
```

## Parameters 

`completion`  

The system calls this handler after the system finishes dismissing the popover.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func dismissPopover() async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

