

- Media Accessibility
-  MACaptionAppearanceCopyBackgroundColor(\_:\_:) 

Function

# MACaptionAppearanceCopyBackgroundColor(\_:\_:)

Returns the preference for the text highlight color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
func MACaptionAppearanceCopyBackgroundColor(
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

The preferred color shown behind the text and above the window color.

## See Also

### Text highlight settings

func MACaptionAppearanceGetBackgroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for the text highlight opacity.

