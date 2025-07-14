

- Media Accessibility
-  MACaptionAppearanceGetWindowRoundedCornerRadius(\_:\_:) 

Function

# MACaptionAppearanceGetWindowRoundedCornerRadius(\_:\_:)

Returns the radius of the caption window’s corners.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceGetWindowRoundedCornerRadius(
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

The system setting for the caption window’s corner radius.

## Discussion

The rounded corners of the caption window are not customizable within the Accessibility preferences and do not change based on text size.

## See Also

### Caption window settings

func MACaptionAppearanceCopyWindowColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for the caption window’s color.

func MACaptionAppearanceGetWindowOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for the overlay’s opacity.

