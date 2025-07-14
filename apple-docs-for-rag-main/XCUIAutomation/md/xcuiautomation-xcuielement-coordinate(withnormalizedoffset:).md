

- XCUIAutomation
- XCUIElement
-  coordinate(withNormalizedOffset:) 

Instance Method

# coordinate(withNormalizedOffset:)

Creates and returns a new coordinate with a normalized offset.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func coordinate(withNormalizedOffset normalizedOffset: CGVector) -> XCUICoordinate
```

## Discussion

The coordinate’s screen point is computed by adding `normalizedOffset` multiplied by the size of the element’s frame to the origin of the element’s frame.

