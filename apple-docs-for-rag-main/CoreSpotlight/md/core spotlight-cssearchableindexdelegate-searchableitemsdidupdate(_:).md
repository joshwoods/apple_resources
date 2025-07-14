

- Core Spotlight
- CSSearchableIndexDelegate
-  searchableItemsDidUpdate(\_:) 

Instance Method

# searchableItemsDidUpdate(\_:)

Tells the delegate that the framework updated the list of searchable items.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
optional func searchableItemsDidUpdate(_ items: [CSSearchableItem])
```

## Parameters 

`items`  

The items the framework updated.

## Discussion

The framework calls this method when it updates an item with specific attributes; see CSSearchableItem.UpdateListenerOptions for Apple Intelligence attributes.

