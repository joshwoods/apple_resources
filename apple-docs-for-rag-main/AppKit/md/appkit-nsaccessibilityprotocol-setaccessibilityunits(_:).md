

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityUnits(\_:) 

Instance Method

# setAccessibilityUnits(\_:)

Sets the units used for the ruler.

macOS 10.10+

``` source
func setAccessibilityUnits(_ accessibilityUnits: NSAccessibilityUnits)
```

**Required**

## See Also

### Configuring Ruler Views

func accessibilityMarkerGroupUIElement() -> Any?

Returns the user interface element that functions as a marker group for the ruler accessibility element.

**Required**

func setAccessibilityMarkerGroupUIElement(Any?)

Sets the user interface element that functions as a marker group for the ruler accessibility element.

**Required**

func accessibilityMarkerTypeDescription() -> String?

Returns the human-readable description of the marker type.

**Required**

func setAccessibilityMarkerTypeDescription(String?)

Sets the human-readable description of the marker type.

**Required**

func accessibilityMarkerUIElements() -> [Any]?

Returns the array of marker accessibility elements for the ruler.

**Required**

func setAccessibilityMarkerUIElements([Any]?)

Sets the array of marker accessibility elements for the ruler.

**Required**

func accessibilityMarkerValues() -> Any?

Returns the marker values for the ruler.

**Required**

func setAccessibilityMarkerValues(Any?)

Sets the marker values for the ruler.

**Required**

func accessibilityRulerMarkerType() -> NSAccessibilityRulerMarkerType

Returns the type of markers for the ruler.

**Required**

func setAccessibilityRulerMarkerType(NSAccessibilityRulerMarkerType)

Sets the type of markers for the ruler.

**Required**

func accessibilityUnits() -> NSAccessibilityUnits

Returns the units for the ruler.

**Required**

func accessibilityUnitDescription() -> String?

Returns the human-readable description of the ruler’s units.

**Required**

func setAccessibilityUnitDescription(String?)

Sets the human-readable description of the ruler’s units.

**Required**

enum NSAccessibilityRulerMarkerType

Values that indicate the marker type of an accessibility element.

enum NSAccessibilityUnits

Values that indicate the unit values of a ruler or layout area.

