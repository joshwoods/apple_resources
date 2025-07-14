

- Foundation
- NSAttributedString
-  boundingRect(with:options:context:) 

Instance Method

# boundingRect(with:options:context:)

Returns the bounding rectangle necessary to draw the string.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func boundingRect(
    with size: CGSize,
    options: NSStringDrawingOptions = [],
    context: NSStringDrawingContext?
) -> CGRect
```

**macOS**

``` source
func boundingRect(
    with size: CGSize,
    options: NSString.DrawingOptions = [],
    context: NSStringDrawingContext?
) -> CGRect
```

## Parameters 

`size`  

The width and height constraints to apply when computing the string’s bounding rectangle.

`options`  

Additional drawing options to apply to the string during rendering. For a list of possible values, see NSStringDrawingOptions.

`context`  

A context object with information about how to adjust the font tracking and scaling information. On return, the specified object contains information about the actual values used to render the string. This parameter may be `nil`.

## Return Value

A rectangle whose size component indicates the width and height required to draw the entire contents of the string.

## Discussion

You can use this method to compute the space required to draw the string. The constraints you specify in the size parameter are a guide for the renderer for how to size the string. However, the actual bounding rectangle returned by this method can be larger than the constraints if additional space is needed to render the entire string. Typically, the renderer preserves the width constraint and adjusts the height constraint as needed.

In iOS 7 and later, this method returns fractional sizes (in the `size` component of the returned rectangle); to use a returned size to size views, you must use raise its value to the nearest higher integer using the ceil function.

### Special Considerations

To calculate the bounding rectangle, this method uses the baseline origin by default, so it behaves as a single line. To render the string in multiple lines, specify usesLineFragmentOrigin in `options`.

## See Also

### Getting metrics for the string

func size() -> CGSize

Returns the size necessary to draw the string.

func containsAttachments(in: NSRange) -> Bool

Returns a Boolean value that indicates if the attributed string contains an attachment in the specified range.

