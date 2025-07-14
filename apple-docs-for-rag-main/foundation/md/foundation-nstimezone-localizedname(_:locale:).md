

- Foundation
- NSTimeZone
-  localizedName(\_:locale:) 

Instance Method

# localizedName(\_:locale:)

Returns the localized name of the time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func localizedName(
    _ style: NSTimeZone.NameStyle,
    locale: Locale?
) -> String?
```

## Parameters 

`style`  

The format style for the returned string.

`locale`  

The locale for which to format the name.

## Return Value

The name of the receiver localized for `locale` using `style`.

## See Also

### Describing Time Zones

var description: String

