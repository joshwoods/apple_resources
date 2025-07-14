

- WidgetKit
- WidgetCenter
-  invalidateRelevance(ofKind:) 

Instance Method

# invalidateRelevance(ofKind:)

Mark the relevance for a kind as invalid.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func invalidateRelevance(ofKind kind: String)
```

## Parameters 

`kind`  

A string that identifies the widget and matches the value you used when you created the widget’s configuration.

## Discussion

Call this function when the relevance returned for a widget has changed and needs to be reloaded.

Marking relevance as invalid will cause the system to call, at a later time, the `relevance` function on the timeline provider that match the specified kind.

