

- Media Accessibility
-  MACaptionAppearanceGetForegroundOpacity(\_:\_:) 

Function

# MACaptionAppearanceGetForegroundOpacity(\_:\_:)

Returns the preference for text opacity.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceGetForegroundOpacity(
    _ domain: MACaptionAppearanceDomain,
    _ behavior: UnsafeMutablePointer?
) -> CGFloat
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

`behavior`  

A pointer to memory. On return, this memory holds the caption appearance behavior for this preference setting. For possible values see MACaptionAppearanceBehavior. Pass `NULL` when you do not need the behavior setting.

## Return Value

The float value, ranging from `0.0` to `1.0`, representing the opacity of the color for text opacity.

## See Also

### Text settings

func MACaptionAppearanceCopyFontDescriptorForStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?, MACaptionAppearanceFontStyle) -> Unmanaged&lt;CTFontDescriptor>

Returns the preferred font for the specified style of type.

func MACaptionAppearanceCopyForegroundColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for text color.

func MACaptionAppearanceGetRelativeCharacterSize(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for font scaling.

func MACaptionAppearanceGetTextEdgeStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> MACaptionAppearanceTextEdgeStyle

Returns the preference for text edge style.

