

- Contacts UI
-  CNContactViewControllerDelegate 

Protocol

# CNContactViewControllerDelegate

Methods you use to respond to user interactions with a contact view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
protocol CNContactViewControllerDelegate : NSObjectProtocol
```

## Overview

Implement the methods of this protocol and assign the resulting object to the delegate property of a `CNContactViewController` object.

## Topics

### Responding to User Events

func contactViewController(CNContactViewController, shouldPerformDefaultActionFor: CNContactProperty) -> Bool

Called when the user selects a property.

func contactViewController(CNContactViewController, didCompleteWith: CNContact?)

Called when the view has been presented.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling Interactions with the Interface

var delegate: (any CNContactViewControllerDelegate)?

The delegate to be notified.

