

- AppKit
- NSTextView
-  changeLayoutOrientation(\_:) 

Instance Method

# changeLayoutOrientation(\_:)

An action method that sets the layout orientation of the text.

macOS 10.7+

``` source
@MainActor
func changeLayoutOrientation(_ sender: Any?)
```

## Parameters 

`sender`  

The sender.

## Discussion

Calls setLayoutOrientation(_:) with the sender’s tag as the orientation.

## See Also

### Changing layout orientation

func setLayoutOrientation(NSLayoutManager.TextLayoutOrientation)

Changes the receiver’s layout orientation and invalidates the contents.

