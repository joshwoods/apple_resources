

- App Intents
- DisplayRepresentation
-  synonyms 

Instance Property

# synonyms

A list of localized phrases that are synonyms of this particular display representation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var synonyms: [LocalizedStringResource]
```

## Discussion

Example:

```
DisplayRepresentation(
    name: "Pizza",
    synonyms: ["Pie", "Za"]
)
```

In this case, “Pie”, “Za” and “Pizza” are all ways to display this

