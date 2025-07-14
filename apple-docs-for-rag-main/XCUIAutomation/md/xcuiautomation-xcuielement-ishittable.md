

- XCUIAutomation
- XCUIElement
-  isHittable 

Instance Property

# isHittable

Determines if the system can compute a hit point for the element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var isHittable: Bool { get }
```

## Discussion

isHittable returns true if the element exists and can be clicked, tapped, or pressed at its current location. It returns false if the element doesn’t exist, is offscreen, or is covered by another element.

Note

isHittable only returns true if the element is already visible and hittable onscreen. It returns false for an offscreen element in a scrollable view, even if the element can be scrolled into a hittable position by calling click(), tap(), or another hit-point-related interaction method.

## See Also

### Querying element state

func waitForExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to exist.

func waitForNonExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to no longer exist.

func wait&lt;V>(for: KeyPath&lt;XCUIElement, V>, toEqual: V, timeout: TimeInterval) -> Bool

Waits a specified amount of time for a property value to equal a specified value.

var exists: Bool

Determines if the element exists.

var debugDescription: String

Provides debugging information about the element.

