

- XCUIAutomation
- XCUIElement
-  exists 

Instance Property

# exists

Determines if the element exists.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var exists: Bool { get }
```

## Discussion

This property determines if the element exists within the app’s current UI hierarchy.

Note

The fact that an element exists doesn’t imply that it’s hittable. Elements can exist offscreen, or exist onscreen but be hidden by another element, causing their isHittable property to return false.

## See Also

### Querying element state

func waitForExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to exist.

func waitForNonExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to no longer exist.

func wait&lt;V>(for: KeyPath&lt;XCUIElement, V>, toEqual: V, timeout: TimeInterval) -> Bool

Waits a specified amount of time for a property value to equal a specified value.

var isHittable: Bool

Determines if the system can compute a hit point for the element.

var debugDescription: String

Provides debugging information about the element.

