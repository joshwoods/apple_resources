

- WidgetKit
-  ActivityViewContext 

Structure

# ActivityViewContext

A structure that describes the view context for creating the views of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
struct ActivityViewContext where Attributes : ActivityAttributes
```

## Topics

### Describing a Live Activity

let attributes: Attributes

A set of attributes that describe a Live Activity and its content at the time of its creation.

let state: Attributes.ContentState

The dynamic content of a Live Activity at the time of its creation.

let isStale: Bool

A Boolean value that describes whether the Live Activity is out of date.

let activityID: String

A unique identifier for the Live Activity.

## See Also

### Creating a Live Activity configuration

init&lt;Content>(for: Attributes.Type, content: (ActivityViewContext&lt;Attributes>) -> Content, dynamicIsland: (ActivityViewContext&lt;Attributes>) -> DynamicIsland)

Creates a configuration object for a Live Activity.

