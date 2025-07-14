

- AppKit
- NSAccessibilityNavigableStaticText
-  accessibilityLine(for:) 

Instance Method

# accessibilityLine(for:)

Returns the line number for the line that contains the specified character index.

macOS

``` source
func accessibilityLine(for index: Int) -> Int
```

**Required**

## Parameters 

`index`  

The index for a character.

## Return Value

The line number for the line holding the specified character index.

## See Also

### Supporting Accessibility

func accessibilityFrame(for: NSRange) -> NSRect

Returns the rectangle that encloses the specified range of characters.

**Required**

func accessibilityRange(forLine: Int) -> NSRange

Returns the range of characters in the specified line.

**Required**

func accessibilityString(for: NSRange) -> String?

Returns the substring for the specified range.

**Required**

