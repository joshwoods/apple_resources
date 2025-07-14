

- WatchKit
-  WKInterfacePaymentButton 

Class

# WKInterfacePaymentButton

A button that you can use to trigger payments through Apple Pay.

watchOS 3.0+

``` source
class WKInterfacePaymentButton
```

## Overview

Use a payment button to initiate an Apple Pay transaction on Apple Watch.

Note

The payment button (see Figure 1) does not create or process payments. It simply provides a button with the Apple Pay mark. You must connect this button to an action method that creates an Apple Pay payment request. For more information on using the Apple Pay mark, see Apple Pay Identity Guidelines.

Do not subclass or create instances of this class yourself. Instead, drag a Payment Button object from your Object Library and add it to your storyboard. Then define an outlet in your interface controller class and connect it to the payment button object.

- Swift
- Objective-C

```
@IBOutlet weak var paymentButton: WKInterfacePaymentButton!
```

```
@property (weak, nonatomic) IBOutlet WKInterfacePaymentButton* paymentButton;
```

During the initialization of your interface controller, WatchKit creates a new instance of this class and assigns it to your outlet. At that point, you can use the object in your outlet to make changes to the payment button. This class does not provide any new public methods or properties. However, it does inherit the methods and properties of its superclass, the WKInterfaceObject class.

To respond to taps in the payment button, declare a method of this form in the interface controller class that manages the button:

- Swift
- Objective-C

```
@IBAction func beginApplePayTransaction()
```

```
- (IBAction)beginApplePayTransaction
```

You can change the name of your action method to anything you like. In your Xcode storyboard, connect the button’s selector to the custom action method defined in your class. In the action method, create the payment request and present the payment sheet by calling a PKPaymentAuthorizationController object’s present(completion:) method.

Payment buttons can be used only to initiate Apple Pay transactions.

## Topics

### Initializing for SwiftUI

init(target: Any?, action: Selector)

Creates a payment button for use in SwiftUI.

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Controls

class WKInterfaceLabel

An interface element that displays static text.

class WKInterfaceDate

A label that displays the current date or time.

class WKInterfaceTimer

A label that displays a countdown or count-up timer.

class WKInterfaceButton

A button in the user interface of your watchOS app.

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

class WKInterfaceTextField

An interface element that displays an editable text area.

class WKInterfaceSwitch

An interface element that toggles between an On and Off state.

class WKInterfaceSlider

An interface element that lets users select a single floating-point value from a range of values.

class WKInterfaceActivityRing

A view that displays data from a HealthKit activity summary object.

class WKInterfaceMap

An interface element that displays a noninteractive map for the location you specify.

