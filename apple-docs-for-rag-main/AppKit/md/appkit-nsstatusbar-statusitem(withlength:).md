

- AppKit
- NSStatusBar
-  statusItem(withLength:) 

Instance Method

# statusItem(withLength:)

Returns a newly created status item that has been allotted a specified space within the status bar.

macOS

``` source
func statusItem(withLength length: CGFloat) -> NSStatusItem
```

## Parameters 

`length`  

A constant that specifies whether the status item is of fixed width, or variable width. The valid constants are described in Status Bar Item Length.

## Return Value

An NSStatusItem object.

## Discussion

The receiver does not retain a reference to the status item, so you need to retain it. Otherwise, the object is removed from the status bar when it is deallocated.

## See Also

### Managing Status items

func removeStatusItem(NSStatusItem)

Removes the specified status item from the receiver.

