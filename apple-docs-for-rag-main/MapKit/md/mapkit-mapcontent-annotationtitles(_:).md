

- MapKit
- MapContent
-  annotationTitles(\_:) 

Instance Method

# annotationTitles(\_:)

Sets the visibility of titles for markers and annotations.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func annotationTitles(_ visibility: Visibility) -> some MapContent
```

## Parameters 

`visibility`  

One of the Visibility settings. The default is Visibility.automatic visibility, that results in the title always being visible.

## Return Value

Returns MapContent whose titles have the visibility setting you specified.

## See Also

### Supplying annotation titles

func annotationSubtitles(Visibility) -> some MapContent

Sets the visibility of subtitles for markers and annotations.

