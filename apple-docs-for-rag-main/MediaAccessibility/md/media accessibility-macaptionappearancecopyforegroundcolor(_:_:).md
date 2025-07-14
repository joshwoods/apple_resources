

- Media Accessibility
-  MACaptionAppearanceCopyForegroundColor(\_:\_:) 

Function

# MACaptionAppearanceCopyForegroundColor(\_:\_:)

Returns the preference for text color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopyForegroundColor(
    _ domain: MACaptionAppearanceDomain,
    _ behavior: UnsafeMutablePointer?
) -> Unmanaged
```

## Parameters 

`domain`  

The domain to retrieve the preference value from. See MACaptionAppearanceDomain. Pass MACaptionAppearanceDomain.user unless the system defaults are needed for comparison.

`behavior`  

A pointer to memory. On return, this memory holds the caption appearance behavior for this preference setting. For possible values see MACaptionAppearanceBehavior. Pass `NULL` when you do not need the behavior setting.

## Return Value

The preferred color for caption text.

## See Also

### Text settings

func MACaptionAppearanceCopyFontDescriptorForStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?, MACaptionAppearanceFontStyle) -> Unmanaged&lt;CTFontDescriptor>

Returns the preferred font for the specified style of type.

func MACaptionAppearanceGetForegroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for text opacity.

func MACaptionAppearanceGetRelativeCharacterSize(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for font scaling.

func MACaptionAppearanceGetTextEdgeStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> MACaptionAppearanceTextEdgeStyle

Returns the preference for text edge style.

