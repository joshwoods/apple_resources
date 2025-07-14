

- Core Spotlight
- CSSearchableItem
-  init(appEntity:priority:) 

Initializer

# init(appEntity:priority:)

Intializes a new searchable item with the relevant fields populated from the provided app entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
convenience init(
    appEntity: Entity,
    priority: Int
) where Entity : IndexedEntity
```

## Parameters 

`appEntity`  

The app entity to use for initialization.

`priority`  

The importance of this item compared to the other donated items.

