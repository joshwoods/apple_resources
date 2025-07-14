

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityDisclosed(\_:) 

Instance Method

# setAccessibilityDisclosed(\_:)

Sets a Boolean value that determines whether the row is disclosing other rows.

macOS 10.10+

``` source
func setAccessibilityDisclosed(_ accessibilityDisclosed: Bool)
```

**Required**

## See Also

### Configuring Outline Rows

func isAccessibilityDisclosed() -> Bool

Returns a Boolean value that determines whether the row is disclosing other rows.

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

func setAccessibilityDisclosureLevel(Int)

Sets the indention level for the row.

**Required**

