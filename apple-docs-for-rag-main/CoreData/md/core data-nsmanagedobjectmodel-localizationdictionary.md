

- Core Data
- NSManagedObjectModel
-  localizationDictionary 

Instance Property

# localizationDictionary

The localization dictionary of the model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var localizationDictionary: [String : String]? { get set }
```

## Discussion

The following table describes the key and value pattern for the localization dictionary.

| Key | Value | Note |
|----|----|----|
| “Entity/NonLocalizedEntityName” | “LocalizedEntityName” |  |
| “Property/NonLocalizedPropertyName/Entity/EntityName” | “LocalizedPropertyName” | \(1\) |
| “Property/NonLocalizedPropertyName” | “LocalizedPropertyName” |  |
| “ErrorString/NonLocalizedErrorString” | “LocalizedErrorString” |  |

\(1\) For properties in different entities with the same non-localized name but that should have different localized names.

### Special Considerations

In OS X v10.4, `localizationDictionary` may return `nil` until Core Data lazily loads the dictionary for its own purposes (for example, reporting a localized error).

