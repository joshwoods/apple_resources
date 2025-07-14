

- AppKit
- NSAccessibilityNavigableStaticText
-  accessibilityString(for:) 

Instance Method

# accessibilityString(for:)

Returns the substring for the specified range.

macOS

``` source
func accessibilityString(for range: NSRange) -> String?
```

**Required**

## Parameters 

`range`  

A range of characters contained by this element.

## Return Value

The substring specified by the given range.

## See Also

### Supporting Accessibility

func accessibilityFrame(for: NSRange) -> NSRect

Returns the rectangle that encloses the specified range of characters.

**Required**

func accessibilityLine(for: Int) -> Int

Returns the line number for the line that contains the specified character index.

**Required**

func accessibilityRange(forLine: Int) -> NSRange

Returns the range of characters in the specified line.

**Required**

