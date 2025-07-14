

- WidgetKit
- WidgetRelevanceGroup
-  ungrouped 

Type Property

# ungrouped

The system may provide a default grouping mechanism, such as per-app grouping, by default.Utilizing the `.ungrouped` option opts out of the default group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
static let ungrouped: WidgetRelevanceGroup
```

## Discussion

Associating `.ungrouped` with a widget alongside other groups has undefined behavior.

