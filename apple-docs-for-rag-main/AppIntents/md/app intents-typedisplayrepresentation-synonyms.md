

- App Intents
- TypeDisplayRepresentation
-  synonyms 

Instance Property

# synonyms

A list of localized phrases that are synonyms of this particular type display representation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var synonyms: [LocalizedStringResource]
```

## Discussion

Example:

```
struct PizzaEntity: AppEntity {
    static var typeDisplayRepresentation = TypeDisplayRepresentation(
        name: "Pizza",
        synonyms: ["Pie", "Za"]
    )
}

```

In this case, we are saying that PizzaEntity can be represented as “Pizza”, “Pie” or “Za”

