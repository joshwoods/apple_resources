

- UIKit
-  UIToolTipInteraction 

Class

# UIToolTipInteraction

An interaction object that makes it possible to show a tooltip when hovering a pointer over a view or control.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UIToolTipInteraction
```

## Overview

To show a tooltip when the pointer hovers over a view, add a UIToolTipInteraction object to the view. For example, the following code listings shows how to add a tooltip to a label:

```
let label = UILabel()
label.text = "Label with a tooltip"

let tooltipInteraction = UIToolTipInteraction(defaultToolTip: "The label's tooltip.")
label.addInteraction(tooltipInteraction)
```

If you want your app to determine the tooltip text at a later time — for instance, to reflect the current state of your app — set the interaction’s delegate property to an object that conforms to the UIToolTipInteractionDelegate protocol.

To add a tooltip to a control derived from UIControl, use the convenience property toolTip; for example, to add a tooltip to the button:

```
let button = UIButton(configuration: configuration, primaryAction: action)
button.toolTip = "Click to buy this item. You'll have a chance to change your mind before confirming your purchase."
```

Setting the toolTip property creates a tooltip interaction for the control, which you can retrieve from the toolTipInteraction property.

Note

Tooltips appear when your app runs in macOS or visionOS. To show a tooltip in macOS, your app must be an iPhone or iPad app running on a Mac with Apple silicon, or built with Mac Catalyst.

## Topics

### Creating a tooltip interaction

init()

Creates a tooltip interaction object.

init(defaultToolTip: String)

Creates a tooltip interaction object and sets the default tooltip text.

### Managing the interaction

var isEnabled: Bool

A Boolean value that indicates whether the tooltip interaction is in the enabled state.

var defaultToolTip: String?

The text that appears in a tooltip by default.

### Providing tooltip configurations

var delegate: (any UIToolTipInteractionDelegate)?

An object that provides text that a tooltip displays instead of the default text.

protocol UIToolTipInteractionDelegate

An interface that provides tooltip settings to an interaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Tooltips

Showing help tags for views and controls using tooltip interactions

Explain the purpose of interface elements by showing a tooltip when a person positions the pointer over the element.

protocol UIToolTipInteractionDelegate

An interface that provides tooltip settings to an interaction.

