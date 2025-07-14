

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityOrderedByRow(\_:) 

Instance Method

# setAccessibilityOrderedByRow(\_:)

Sets a Boolean value that determines whether the element’s grid is in row major order or in column major order.

macOS 10.10+

``` source
func setAccessibilityOrderedByRow(_ accessibilityOrderedByRow: Bool)
```

**Required**

## See Also

### Configuring Grid Views

func accessibilityColumnCount() -> Int

Returns the number of columns in the accessibility element’s grid.

**Required**

func setAccessibilityColumnCount(Int)

Sets the number of columns in the accessibility element’s grid.

**Required**

func isAccessibilityOrderedByRow() -> Bool

Returns a Boolean value that determines whether the accessibility element’s grid is in row major order or in column major order.

**Required**

func accessibilityRowCount() -> Int

Returns the number of rows in the accessibility element’s grid.

**Required**

func setAccessibilityRowCount(Int)

Sets the number of rows in the accessibility element’s grid.

**Required**

