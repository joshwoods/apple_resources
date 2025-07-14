

- Application Services
- Carbon Accessibility
-  Actions 

API Collection

# Actions

Define the actions an accessibility object can perform.

## Topics

### Constants

var kAXPressAction: String

Simulates a single click, such as on a button.

var kAXIncrementAction: String

Increments the value of the accessibility object. The amount the value is incremented by is determined by the value of the `kAXValueIncrementAttribute` attribute.

var kAXDecrementAction: String

Decrements the value of the accessibility object. The amount the value is decremented by is determined by the value of the `kAXValueIncrementAttribute` attribute.

var kAXConfirmAction: String

Simulates pressing the Return key.

var kAXCancelAction: String

Simulates pressing a Cancel button.

var kAXRaiseAction: String

Causes a window to become as frontmost as is allowed by the containing application’s circumstances. Note that an application’s floating windows (such as inspector windows) might remain above a window that performs the raise action.

var kAXShowMenuAction: String

## See Also

### Accessibility Object Constants

Roles

Define the values an accessibility object’s role attribute can have.

Subroles

Define the values for an accessibility object’s subrole attribute.

Attributes

Define the attributes available for accessibility objects.

Parameterized Attributes

Define the parameterized attributes an accessibility object can have.

Notifications

Define the notifications that can be broadcast by an accessibility object.

Orientations and Sort Directions

Define the values for the orientation and sort-direction attributes of some accessibility objects.

