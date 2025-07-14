

- UIKit
- UIResponder
-  inputAccessoryView 

Instance Property

# inputAccessoryView

The custom input accessory view to display when the responder becomes the first responder.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var inputAccessoryView: UIView? { get }
```

## Discussion

This property is typically used to attach an accessory view to the system-supplied keyboard that’s presented for UITextField and UITextView objects.

The value of this read-only property is `nil`. If you want to attach custom controls to a system-supplied input view (such as the system keyboard) or to a custom input view (one you provide in the inputView property), redeclare this property as read-write in a UIResponder subclass. You can then use this property to manage a custom accessory view. When the responder becomes the first responder, the responder infrastructure attaches the accessory view to the appropriate input view before displaying it.

This property has special considerations in visionOS:

- In apps built for visionOS, this property isn’t available. Use bottomOrnament instead.

- In compatible iPad and iPhone apps running in visionOS, the app’s idiom determines this property’s behavior. For apps running in the UIUserInterfaceIdiom.pad idiom, the accessory view renders at the bottom of the app window. For apps running in the UIUserInterfaceIdiom.phone idiom, this property doesn’t have any effect.

## See Also

### Managing input views

var inputView: UIView?

The custom input view to display when the responder becomes the first responder.

var inputViewController: UIInputViewController?

The custom input view controller to use when the responder becomes the first responder.

var inputAccessoryViewController: UIInputViewController?

The custom input accessory view controller to display when the responder becomes the first responder.

func reloadInputViews()

Updates the custom input and accessory views when the object is the first responder.

