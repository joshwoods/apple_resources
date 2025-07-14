

- Media Accessibility
-  MACaptionAppearanceGetRelativeCharacterSize(\_:\_:) 

Function

# MACaptionAppearanceGetRelativeCharacterSize(\_:\_:)

Returns the preference for font scaling.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceGetRelativeCharacterSize(
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

The font scaling preference, as a multiplier, for the specified style; ranging from `0.0` to `2.0`.

## See Also

### Text settings

func MACaptionAppearanceCopyFontDescriptorForStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?, MACaptionAppearanceFontStyle) -> Unmanaged&lt;CTFontDescriptor>

Returns the preferred font for the specified style of type.

func MACaptionAppearanceCopyForegroundColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for text color.

func MACaptionAppearanceGetForegroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for text opacity.

func MACaptionAppearanceGetTextEdgeStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> MACaptionAppearanceTextEdgeStyle

Returns the preference for text edge style.

