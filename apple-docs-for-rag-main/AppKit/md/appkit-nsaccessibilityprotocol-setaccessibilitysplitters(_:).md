

- AppKit
- NSAccessibilityProtocol
-  setAccessibilitySplitters(\_:) 

Instance Method

# setAccessibilitySplitters(\_:)

Sets the array that contains the views and splitter bar from the split view.

macOS 10.10+

``` source
func setAccessibilitySplitters(_ accessibilitySplitters: [Any]?)
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

func accessibilitySplitters() -> [Any]?

Returns an array that contains the views and splitter bar from the split view.

**Required**

