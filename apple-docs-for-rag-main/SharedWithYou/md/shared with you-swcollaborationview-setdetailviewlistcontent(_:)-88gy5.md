

- Shared With You
- SWCollaborationView
-  setDetailViewListContent(\_:) 

Instance Method

# setDetailViewListContent(\_:)

Sets the detail view for the list content.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+visionOS

``` source
@MainActor @preconcurrency
func setDetailViewListContent(_ detailViewListContent: ListContent) where ListContent : View
```

## Parameters 

`detailViewListContent`  

A `ListContent` view.

## See Also

### Setting view attributes

func setContent(UIView)

Sets the content view.

func setDetailViewListContent&lt;ListContent>(() -> ListContent)

Sets the detail view for the list content from view builder closures.

func setShowManageButton(Bool)

A Boolean value the system uses to show or hide the default manage-participants button in the collaboration popover.

