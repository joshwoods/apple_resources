

- App Intents
- IndexedEntity
-  defaultAttributeSet 

Instance Property

# defaultAttributeSet

Custom attributes that improve search accuracy in Spotlight.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var defaultAttributeSet: CSSearchableItemAttributeSet { get }
```

## Discussion

Per default, Spotlight search uses the title, subtitle, and image from an entity’s display representation. To allow Spotlight to search other entity attributes and increase search accuracy, provide a set of custom attributes for data you donate.

