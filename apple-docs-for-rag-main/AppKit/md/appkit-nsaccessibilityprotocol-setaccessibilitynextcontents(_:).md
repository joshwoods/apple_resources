

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityNextContents(\_:) 

Instance Method

# setAccessibilityNextContents(\_:)

Sets the contents that follow the divider accessibility element.

macOS 10.10+

``` source
func setAccessibilityNextContents(_ accessibilityNextContents: [Any]?)
```

**Required**

## See Also

### Configuring Split Views

func accessibilityNextContents() -> [Any]?

Returns the contents that follow the divider accessibility element.

**Required**

func accessibilityPreviousContents() -> [Any]?

Returns the contents that precede the divider accessibility element.

**Required**

func setAccessibilityPreviousContents([Any]?)

Sets the contents that precede the divider accessibility element.

**Required**

func accessibilitySplitters() -> [Any]?

Returns an array that contains the views and splitter bar from the split view.

**Required**

func setAccessibilitySplitters([Any]?)

Sets the array that contains the views and splitter bar from the split view.

**Required**

