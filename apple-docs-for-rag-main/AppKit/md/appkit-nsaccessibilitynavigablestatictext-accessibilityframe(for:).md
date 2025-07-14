

- AppKit
- NSAccessibilityNavigableStaticText
-  accessibilityFrame(for:) 

Instance Method

# accessibilityFrame(for:)

Returns the rectangle that encloses the specified range of characters.

macOS

``` source
func accessibilityFrame(for range: NSRange) -> NSRect
```

**Required**

## Parameters 

`range`  

The range of characters.

## Return Value

The rectangle that encloses the specified characters.

## Discussion

If the range crosses a line boundary, the returned rectangle will fully enclose all the lines of characters.

## See Also

### Supporting Accessibility

func accessibilityLine(for: Int) -> Int

Returns the line number for the line that contains the specified character index.

**Required**

func accessibilityRange(forLine: Int) -> NSRange

Returns the range of characters in the specified line.

**Required**

func accessibilityString(for: NSRange) -> String?

Returns the substring for the specified range.

**Required**

