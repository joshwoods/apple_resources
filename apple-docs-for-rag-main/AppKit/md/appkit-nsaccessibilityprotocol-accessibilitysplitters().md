

- AppKit
- NSAccessibilityProtocol
-  accessibilitySplitters() 

Instance Method

# accessibilitySplitters()

Returns an array that contains the views and splitter bar from the split view.

macOS 10.10+

``` source
func accessibilitySplitters() -> [Any]?
```

**Required**

## See Also

### Configuring Split Views

func accessibilityNextContents() -> [Any]?

Returns the contents that follow the divider accessibility element.

**Required**

func setAccessibilityNextContents([Any]?)

Sets the contents that follow the divider accessibility element.

**Required**

func accessibilityPreviousContents() -> [Any]?

Returns the contents that precede the divider accessibility element.

**Required**

func setAccessibilityPreviousContents([Any]?)

Sets the contents that precede the divider accessibility element.

**Required**

func setAccessibilitySplitters([Any]?)

Sets the array that contains the views and splitter bar from the split view.

**Required**

