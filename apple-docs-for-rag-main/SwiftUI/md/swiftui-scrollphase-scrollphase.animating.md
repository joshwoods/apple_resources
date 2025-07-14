

- SwiftUI
- ScrollPhase
-  ScrollPhase.animating 

Case

# ScrollPhase.animating

The animating phase where the scroll view is animating towards a final target.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
case animating
```

## Discussion

This phase is the result of a programmatic scroll when using a ScrollViewReader or scrollPosition(id:anchor:) modifier.

SwiftUI provides you a value of this type when using the onScrollPhaseChange(_:) modifier with a scrollable view like ScrollView or List.

## See Also

### Getting scroll gesture states

case decelerating

The decelerating phase where the user use has stopped interacting with the scroll view and the scroll view is decelerating towards its final target.

case idle

The idle phase where no kind of scrolling is occurring.

case interacting

The interacting phase where the user is interacting with the scroll view.

case tracking

The tracking phase where the scroll view is tracking a potential scroll by the user but the user hasn’t started a scroll.

