

- Media Accessibility
-  MACaptionAppearanceCopyFontDescriptorForStyle(\_:\_:\_:) 

Function

# MACaptionAppearanceCopyFontDescriptorForStyle(\_:\_:\_:)

Returns the preferred font for the specified style of type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopyFontDescriptorForStyle(
    _ domain: MACaptionAppearanceDomain,
    _ behavior: UnsafeMutablePointer?,
    _ fontStyle: MACaptionAppearanceFontStyle
) -> Unmanaged
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

`behavior`  

A pointer to memory. On return, this memory holds the caption appearance behavior for this preference setting. For possible values see MACaptionAppearanceBehavior. Pass `NULL` when you do not need the behavior setting.

`fontStyle`  

A font style, such as cursive or small caps, see MACaptionAppearanceFontStyle.

## Return Value

The name of the preferred font for the specified style.

## See Also

### Text settings

func MACaptionAppearanceCopyForegroundColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for text color.

func MACaptionAppearanceGetForegroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for text opacity.

func MACaptionAppearanceGetRelativeCharacterSize(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for font scaling.

func MACaptionAppearanceGetTextEdgeStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> MACaptionAppearanceTextEdgeStyle

Returns the preference for text edge style.

