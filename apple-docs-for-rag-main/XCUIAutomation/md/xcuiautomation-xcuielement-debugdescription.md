

- XCUIAutomation
- XCUIElement
-  debugDescription 

Instance Property

# debugDescription

Provides debugging information about the element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var debugDescription: String { get }
```

## Discussion

The data in the string varies based on the time at which it’s captured, but it may include any of the following, as well as additional data:

- Values for the element’s attributes

- The entire tree of descendants rooted at the element

- The element’s query

Use this data for debugging only. Depending on any of the data as part of a test is unsupported.

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

var isHittable: Bool

Determines if the system can compute a hit point for the element.

