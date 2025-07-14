

- AppKit
- NSAccessibilityProtocol
-  accessibilityLayoutPoint(forScreenPoint:) 

Instance Method

# accessibilityLayoutPoint(forScreenPoint:)

Converts the provided point in screen coordinates to a point in the layout area’s coordinate system.

macOS 10.10+

``` source
func accessibilityLayoutPoint(forScreenPoint point: NSPoint) -> NSPoint
```

**Required**

## Parameters 

`point`  

A point in the screen’s coordinate system.

## Return Value

A point in the layout area’s coordinate system.

## See Also

### Configuring Layout

func accessibilityHandles() -> [Any]?

Returns the drag handle elements for the layout item element.

**Required**

func setAccessibilityHandles([Any]?)

Sets the drag handle accessibility elements for the layout item element.

**Required**

func accessibilityHorizontalUnits() -> NSAccessibilityUnits

Returns the units that the layout area uses for horizontal values.

**Required**

func setAccessibilityHorizontalUnits(NSAccessibilityUnits)

Sets the units that the layout area uses for horizontal values.

**Required**

func accessibilityHorizontalUnitDescription() -> String?

Returns the description of the layout area’s horizontal units.

**Required**

func setAccessibilityHorizontalUnitDescription(String?)

Sets the description of the layout area’s horizontal units.

**Required**

func accessibilityVerticalUnits() -> NSAccessibilityUnits

Returns the units that the layout area uses for vertical values.

**Required**

func setAccessibilityVerticalUnits(NSAccessibilityUnits)

Sets the units that the layout area uses for vertical values.

**Required**

func accessibilityVerticalUnitDescription() -> String?

Returns the description of the layout area’s vertical units.

**Required**

func setAccessibilityVerticalUnitDescription(String?)

Sets the description of the layout area’s vertical units.

**Required**

func accessibilityLayoutSize(forScreenSize: NSSize) -> NSSize

Converts the provided size in screen coordinates to a size in the layout area’s coordinate system.

**Required**

func accessibilityScreenPoint(forLayoutPoint: NSPoint) -> NSPoint

Converts the provided point in the layout area’s coordinates to a point in the screen’s coordinate system.

**Required**

func accessibilityScreenSize(forLayoutSize: NSSize) -> NSSize

Converts the provided size in the layout area’s coordinates to a size in the screen’s coordinate system.

**Required**

