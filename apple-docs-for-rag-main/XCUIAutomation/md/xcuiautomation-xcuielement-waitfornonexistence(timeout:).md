

- XCUIAutomation
- XCUIElement
-  waitForNonExistence(timeout:) 

Instance Method

# waitForNonExistence(timeout:)

Waits the specified amount of time for an element to no longer exist.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func waitForNonExistence(timeout: TimeInterval) -> Bool
```

## Parameters 

`timeout`  

The time, in seconds, the test allows for the element to become unavailable. The default timeout allows the test to run until it reaches its execution time allowance.

## Discussion

## See Also

### Querying element state

func waitForExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to exist.

func wait&lt;V>(for: KeyPath&lt;XCUIElement, V>, toEqual: V, timeout: TimeInterval) -> Bool

Waits a specified amount of time for a property value to equal a specified value.

var exists: Bool

Determines if the element exists.

var isHittable: Bool

Determines if the system can compute a hit point for the element.

var debugDescription: String

Provides debugging information about the element.

