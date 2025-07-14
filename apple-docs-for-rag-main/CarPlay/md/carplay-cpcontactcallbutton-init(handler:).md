

- CarPlay
- CPContactCallButton
-  init(handler:) 

Initializer

# init(handler:)

Creates a button that invokes a handler when the user taps it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(handler: ((CPButton) -> Void)? = nil)
```

## Parameters 

`handler`  

The closure that the button invokes when the user taps it.

## Return Value

A new contact directions button that invokes its handler when the user taps it.

## Discussion

The button displays a system image that communicates its function.

