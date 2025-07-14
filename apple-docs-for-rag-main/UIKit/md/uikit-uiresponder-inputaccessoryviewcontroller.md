

- UIKit
- UIResponder
-  inputAccessoryViewController 

Instance Property

# inputAccessoryViewController

The custom input accessory view controller to display when the responder becomes the first responder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var inputAccessoryViewController: UIInputViewController? { get }
```

## Discussion

This property is typically used to attach an accessory view controller to the system-supplied keyboard that’s presented for UITextField and UITextView objects.

The value of this read-only property is `nil`. If you want to attach custom controls to a system-supplied input view controller (such as the system keyboard) or to a custom input view (one you provide in the inputViewController property), redeclare this property as read-write in a UIResponder subclass. You can then use this property to manage a custom accessory view. When the responder becomes the first responder, the responder infrastructure attaches the accessory view to the appropriate input view before displaying it.

## See Also

### Managing input views

var inputView: UIView?

The custom input view to display when the responder becomes the first responder.

var inputViewController: UIInputViewController?

The custom input view controller to use when the responder becomes the first responder.

var inputAccessoryView: UIView?

The custom input accessory view to display when the responder becomes the first responder.

func reloadInputViews()

Updates the custom input and accessory views when the object is the first responder.

