

- App Intents
- IndexedEntity
-  attributeSet 

Instance Property

# attributeSet

Provide a customized attribute set for improved search accuracy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var attributeSet: CSSearchableItemAttributeSet { get }
```

**Required** Default implementation provided.

## Discussion

The default implementation uses the title, subtitle and image from the display representation.

## Default Implementations

### IndexedEntity Implementations

var attributeSet: CSSearchableItemAttributeSet

Provide a customized attribute set for improved search accuracy.

