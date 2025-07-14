

- AppKit
- NSAccessibilityNavigableStaticText
-  accessibilityRange(forLine:) 

Instance Method

# accessibilityRange(forLine:)

Returns the range of characters in the specified line.

macOS

``` source
func accessibilityRange(forLine lineNumber: Int) -> NSRange
```

**Required**

## Parameters 

`lineNumber`  

The line number to be examined.

## Return Value

The range of characters for the specified line number. If the line ends with a newline character, including the newline is preferred.

## See Also

### Supporting Accessibility

func accessibilityFrame(for: NSRange) -> NSRect

Returns the rectangle that encloses the specified range of characters.

**Required**

func accessibilityLine(for: Int) -> Int

Returns the line number for the line that contains the specified character index.

**Required**

func accessibilityString(for: NSRange) -> String?

Returns the substring for the specified range.

**Required**

