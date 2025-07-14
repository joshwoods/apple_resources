

- Core Text
-  CTParagraphStyleCreateCopy(\_:) 

Function

# CTParagraphStyleCreateCopy(\_:)

Creates an immutable copy of a paragraph style.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTParagraphStyleCreateCopy(_ paragraphStyle: CTParagraphStyle) -> CTParagraphStyle
```

## Parameters 

`paragraphStyle`  

The style to copy. This parameter may not be `NULL`.

## Return Value

A valid reference to an immutable CTParagraphStyle object that is a copy of the one passed into `paragraphStyle`, If the `paragraphStyle` reference is valid; otherwise `NULL`, if any error occurred, including being supplied with an invalid reference.

## See Also

### Creating Paragraph Styles

func CTParagraphStyleCreate(UnsafePointer&lt;CTParagraphStyleSetting>?, Int) -> CTParagraphStyle

Creates an immutable paragraph style.

