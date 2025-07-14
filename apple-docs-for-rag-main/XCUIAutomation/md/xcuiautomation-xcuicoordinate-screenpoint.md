

- XCUIAutomation
- XCUICoordinate
-  screenPoint 

Instance Property

# screenPoint

The dynamically computed value of the coordinate’s location on screen.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
var screenPoint: CGPoint { get }
```

## Discussion

Note that this value is dependent on the current frame of the referenced element. If the element’s frame changes, so does the value returned by this property. If the referenced element doesn’t exist when you call this property, the system fails the current test. Check the referenced element’s exists property to veryify whether the element is present.

## See Also

### Getting coordinate properties

var referencedElement: XCUIElement

The element that the coordinate is based on, either directly or through the coordinate from which it was derived.

