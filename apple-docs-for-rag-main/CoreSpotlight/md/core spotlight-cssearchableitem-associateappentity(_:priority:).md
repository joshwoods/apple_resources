

- Core Spotlight
- CSSearchableItem
-  associateAppEntity(\_:priority:) 

Instance Method

# associateAppEntity(\_:priority:)

Associates an app entity with this searchable item.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func associateAppEntity(
    _ appEntity: some IndexedEntity,
    priority: Int = 0
)
```

## Parameters 

`appEntity`  

The app entity that will be associated with this searchable item.

`priority`  

The importance of this item compared to the other donated items.

