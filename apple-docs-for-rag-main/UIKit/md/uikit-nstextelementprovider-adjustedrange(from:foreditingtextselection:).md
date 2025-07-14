

- UIKit
- NSTextElementProvider
-  adjustedRange(from:forEditingTextSelection:) 

Instance Method

# adjustedRange(from:forEditingTextSelection:)

A method you implement if the location backing store requires manual adjustment after editing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
optional func adjustedRange(
    from textRange: NSTextRange,
    forEditingTextSelection: Bool
) -> NSTextRange?
```

## Parameters 

`textRange`  

An NSTextRange that the method adjusts.

`forEditingTextSelection`  

A Boolean value that indicates if `textRange` is for the text selection associated with the edit session.

## Return Value

When `textRange` is intersecting or following the current edited range, the method returns the range adjusted for the modification in the editing session. Returns `nil`, when no adjustment necessary.

## See Also

### Adjusting the range of the text element

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the offset between the two specified locations.

