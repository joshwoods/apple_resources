

- Shared With You
- SWHighlightCenterDelegate
-  highlightCenterHighlightsDidChange(\_:) 

Instance Method

# highlightCenterHighlightsDidChange(\_:)

Notifies the delegate that the list or rank order of surfaced highlights has changed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func highlightCenterHighlightsDidChange(_ highlightCenter: SWHighlightCenter)
```

**Required**

## Parameters 

`highlightCenter`  

The delegete for the hightlight center.

## Discussion

When the system calls this method, the app updates any displayed highlights to match the updated list. Only the highlights provided by the system should have a shared indication. If no highlights are in the list, the app should remove any links previously indicated.

The array is a priority-ordered list, where the first element in the array is the most relevant to the user. The list of provided highlights is empty if there are no highlights or if the user hasn’t given permission for the app to display highlights.

