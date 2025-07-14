

- WidgetKit
- WidgetCenter
-  reloadTimelines(ofKind:) 

Instance Method

# reloadTimelines(ofKind:)

Reloads the timelines for all widgets of a particular kind.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
func reloadTimelines(ofKind kind: String)
```

## Parameters 

`kind`  

A string that identifies the widget and matches the value you used when you created the widget’s configuration.

## See Also

### Reloading Widget Timelines

func reloadAllTimelines()

Reloads the timelines for all configured widgets belonging to the containing app.

