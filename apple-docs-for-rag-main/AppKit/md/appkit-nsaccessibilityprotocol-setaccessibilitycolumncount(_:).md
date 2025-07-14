

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityColumnCount(\_:) 

Instance Method

# setAccessibilityColumnCount(\_:)

Sets the number of columns in the accessibility element’s grid.

macOS 10.10+

``` source
func setAccessibilityColumnCount(_ accessibilityColumnCount: Int)
```

**Required**

## See Also

### Configuring Grid Views

func accessibilityColumnCount() -> Int

Returns the number of columns in the accessibility element’s grid.

**Required**

func isAccessibilityOrderedByRow() -> Bool

Returns a Boolean value that determines whether the accessibility element’s grid is in row major order or in column major order.

**Required**

func setAccessibilityOrderedByRow(Bool)

Sets a Boolean value that determines whether the element’s grid is in row major order or in column major order.

**Required**

func accessibilityRowCount() -> Int

Returns the number of rows in the accessibility element’s grid.

**Required**

func setAccessibilityRowCount(Int)

Sets the number of rows in the accessibility element’s grid.

**Required**

