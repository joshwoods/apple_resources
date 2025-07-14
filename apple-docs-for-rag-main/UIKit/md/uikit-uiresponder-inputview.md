

- UIKit
- UIResponder
-  inputView 

Instance Property

# inputView

The custom input view to display when the responder becomes the first responder.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var inputView: UIView? { get }
```

## Discussion

This property is typically used to provide a view to replace the system-supplied keyboard that’s presented for UITextField and UITextView objects.

The value of this read-only property is `nil`. A responder object that requires a custom view to gather input from the user should redeclare this property as read-write and use it to manage its custom input view. When the responder becomes the first responder, the responder infrastructure presents the specified input view automatically. Similarly, when the responder resigns its first responder status, the responder infrastructure automatically dismisses the specified input view.

## See Also

### Managing input views

var inputViewController: UIInputViewController?

The custom input view controller to use when the responder becomes the first responder.

var inputAccessoryView: UIView?

The custom input accessory view to display when the responder becomes the first responder.

var inputAccessoryViewController: UIInputViewController?

The custom input accessory view controller to display when the responder becomes the first responder.

func reloadInputViews()

Updates the custom input and accessory views when the object is the first responder.

