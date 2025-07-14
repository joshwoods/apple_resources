

- App Intents
- ParameterSummarySwitchCondition
-  init(\_:\_:) 

Initializer

# init(\_:\_:)

Initializes a parameter summary Switch statement over widget family.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ widgetFamily: ParameterSummarySwitchCondition.WidgetFamily,
    @ParameterSummaryCaseBuilder _ builder: () -> CaseCondition
) where Value == IntentWidgetFamily
```

## Discussion

For example:

```
static var parameterSummary: some ParameterSummary {
    Switch(.widgetFamily) {
        Case(.systemLarge) {
            Summary("Parameter summary for large widgets")
        }
        Case([.systemSmall, .systemMedium]) {
            Summary("Parameter summary for small and medium widgets")
        }
        DefaultCase {
            Summary("Default parameter summary")
        }
    }
}
```

