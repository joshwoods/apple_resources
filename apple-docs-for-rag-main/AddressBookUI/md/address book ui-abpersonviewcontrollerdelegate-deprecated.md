

- Address Book UI
-  ABPersonViewControllerDelegate Deprecated

Protocol

# ABPersonViewControllerDelegate

The `ABPersonViewControllerDelegate` protocol declares the interface that must be implemented by ABPersonViewController delegates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 14.0+

``` source
protocol ABPersonViewControllerDelegate : NSObjectProtocol
```

Deprecated

Use CNContactViewController instead.

## Topics

### Responding to User Events

func personViewController(ABPersonViewController, shouldPerformDefaultActionForPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects a property value of the person displayed in a person view controller.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to View Controller Interactions

var personViewDelegate: (any ABPersonViewControllerDelegate)?

The person-view controller delegate.

Deprecated

