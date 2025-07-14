

- XCUIAutomation
- XCUIElement
-  tap(withNumberOfTaps:numberOfTouches:) 

Instance Method

# tap(withNumberOfTaps:numberOfTouches:)

Sends one or more taps with one or more touch points.

iOSiPadOSMac CatalystwatchOSXcode 16.3+

``` source
@MainActor
func tap(
    withNumberOfTaps numberOfTaps: Int,
    numberOfTouches: Int
)
```

## Parameters 

`numberOfTaps`  

The number of taps.

`numberOfTouches`  

The number of touch points.

## See Also

### Tapping multiple times

func twoFingerTap()

Sends a two-finger tap event to a hittable point the system computes for the element.

