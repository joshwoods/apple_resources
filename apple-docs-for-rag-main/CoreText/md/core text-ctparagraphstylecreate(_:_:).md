

- Core Text
-  CTParagraphStyleCreate(\_:\_:) 

Function

# CTParagraphStyleCreate(\_:\_:)

Creates an immutable paragraph style.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTParagraphStyleCreate(
    _ settings: UnsafePointer?,
    _ settingCount: Int
) -> CTParagraphStyle
```

## Parameters 

`settings`  

The settings with which to preload the paragraph style. If you want to specify the default set of settings, set this parameter to `NULL`.

`settingCount`  

The number of settings that you have specified in the `settings` parameter. This must be greater than or equal to `0`.

## Return Value

A valid reference to an immutable CTParagraphStyle object, If the paragraph style creation was successful; otherwise, `NULL`.

## Discussion

Using this function is the easiest and most efficient way to create a paragraph style. Paragraph styles should be kept immutable for totally lock-free operation. If an invalid paragraph style setting specifier is passed into the `settings` parameter, nothing bad will happen, but you will be unable to query for this value. The reason is to allow backward compatibility with style setting specifiers that may be introduced in future versions.

## See Also

### Creating Paragraph Styles

func CTParagraphStyleCreateCopy(CTParagraphStyle) -> CTParagraphStyle

Creates an immutable copy of a paragraph style.

