

- SwiftUI
- MatchedTransitionSourceConfiguration
-  background(\_:) 

Instance Method

# background(\_:)

Specifies a color that will be drawn behind the content within the matched transition source.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func background(_ style: Color) -> some MatchedTransitionSourceConfiguration
```

## Discussion

During a zoom transition, the background color fills the interpolated shape as it groes from the matched transition source.

