

- UIKit
- UIResponder
-  inputViewController 

Instance Property

# inputViewController

The custom input view controller to use when the responder becomes the first responder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var inputViewController: UIInputViewController? { get }
```

## Discussion

This property is typically used to provide a view controller to replace the system-supplied keyboard that’s presented for UITextField and UITextView objects.

The value of this read-only property is `nil`. If you want to provide a custom input view controller to replace the system keyboard in your app, redeclare this property as read-write in a UIResponder subclass. You can then use this property to manage a custom input view controller. When the responder becomes the first responder, the responder infrastructure presents the specified input view controller automatically. Similarly, when the responder resigns its first responder status, the responder infrastructure automatically dismisses the specified input view controller.

## See Also

### Managing input views

var inputView: UIView?

The custom input view to display when the responder becomes the first responder.

var inputAccessoryView: UIView?

The custom input accessory view to display when the responder becomes the first responder.

var inputAccessoryViewController: UIInputViewController?

The custom input accessory view controller to display when the responder becomes the first responder.

func reloadInputViews()

Updates the custom input and accessory views when the object is the first responder.

