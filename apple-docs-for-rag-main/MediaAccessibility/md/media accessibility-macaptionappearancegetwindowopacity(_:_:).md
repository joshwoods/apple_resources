

- Media Accessibility
-  MACaptionAppearanceGetWindowOpacity(\_:\_:) 

Function

# MACaptionAppearanceGetWindowOpacity(\_:\_:)

Returns the preference for the overlay’s opacity.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceGetWindowOpacity(
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

The float value, ranging from `0.0` to `1.0`, representing the opacity of the color behind all other caption elements.

## See Also

### Caption window settings

func MACaptionAppearanceCopyWindowColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for the caption window’s color.

func MACaptionAppearanceGetWindowRoundedCornerRadius(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the radius of the caption window’s corners.

