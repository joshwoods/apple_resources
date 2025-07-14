

- XCUIAutomation
- XCUIElement
-  waitForExistence(timeout:) 

Instance Method

# waitForExistence(timeout:)

Waits the specified amount of time for an element to exist.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func waitForExistence(timeout: TimeInterval) -> Bool
```

## Discussion

Returns false if the timeout expires while the element’s exists property equals false.

## See Also

### Querying element state

func waitForNonExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to no longer exist.

func wait&lt;V>(for: KeyPath&lt;XCUIElement, V>, toEqual: V, timeout: TimeInterval) -> Bool

Waits a specified amount of time for a property value to equal a specified value.

var exists: Bool

Determines if the element exists.

var isHittable: Bool

Determines if the system can compute a hit point for the element.

var debugDescription: String

Provides debugging information about the element.

