

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityDisclosureLevel(\_:) 

Instance Method

# setAccessibilityDisclosureLevel(\_:)

Sets the indention level for the row.

macOS 10.10+

``` source
func setAccessibilityDisclosureLevel(_ accessibilityDisclosureLevel: Int)
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

func accessibilityDisclosedByRow() -> Any?

Returns the row disclosing the current row.

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

