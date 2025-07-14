

- XCUIAutomation
- XCUIElement
-  wait(for:toEqual:timeout:) 

Instance Method

# wait(for:toEqual:timeout:)

Waits a specified amount of time for a property value to equal a specified value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor @preconcurrency
func wait(
    for keyPath: KeyPath,
    toEqual expectedValue: V,
    timeout: TimeInterval
) -> Bool where V : Equatable
```

## Parameters 

`keyPath`  

The observed property on an XCUIElement.

`expectedValue`  

The desired value, which must conform to `Equatable`.

`timeout`  

The length of time in seconds to wait for the observed property to equal the expected value.

## Discussion

This method returns false if the timeout expires before the observed property equals the expected value.

## See Also

### Querying element state

func waitForExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to exist.

func waitForNonExistence(timeout: TimeInterval) -> Bool

Waits the specified amount of time for an element to no longer exist.

var exists: Bool

Determines if the element exists.

var isHittable: Bool

Determines if the system can compute a hit point for the element.

var debugDescription: String

Provides debugging information about the element.

