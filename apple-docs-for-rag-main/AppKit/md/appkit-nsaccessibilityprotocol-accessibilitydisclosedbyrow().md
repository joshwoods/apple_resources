

- AppKit
- NSAccessibilityProtocol
-  accessibilityDisclosedByRow() 

Instance Method

# accessibilityDisclosedByRow()

Returns the row disclosing the current row.

macOS 10.10+

``` source
func accessibilityDisclosedByRow() -> Any?
```

**Required**

## See Also

### Configuring Outline Rows

func isAccessibilityDisclosed() -> Bool

Returns a Boolean value that determines whether the row is disclosing other rows.

**Required**

func setAccessibilityDisclosed(Bool)

Sets a Boolean value that determines whether the row is disclosing other rows.

**Required**

func setAccessibilityDisclosedByRow(Any?)

Sets the row disclosing the current row.

**Required**

func accessibilityDisclosedRows() -> Any?

Returns the rows that the current row discloses.

**Required**

func setAccessibilityDisclosedRows(Any?)

Sets the rows that the current row discloses.

**Required**

func accessibilityDisclosureLevel() -> Int

Returns the indention level for the row.

**Required**

func setAccessibilityDisclosureLevel(Int)

Sets the indention level for the row.

**Required**

