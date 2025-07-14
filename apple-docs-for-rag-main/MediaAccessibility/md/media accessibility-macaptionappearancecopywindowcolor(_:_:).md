

- Media Accessibility
-  MACaptionAppearanceCopyWindowColor(\_:\_:) 

Function

# MACaptionAppearanceCopyWindowColor(\_:\_:)

Returns the preference for the caption window’s color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopyWindowColor(
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

The preferred color displayed behind all other caption elements.

## See Also

### Caption window settings

func MACaptionAppearanceGetWindowOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for the overlay’s opacity.

func MACaptionAppearanceGetWindowRoundedCornerRadius(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the radius of the caption window’s corners.

