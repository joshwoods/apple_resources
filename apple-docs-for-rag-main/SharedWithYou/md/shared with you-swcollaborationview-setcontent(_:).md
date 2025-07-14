

- Shared With You
- SWCollaborationView
-  setContent(\_:) 

Instance Method

# setContent(\_:)

Sets the content view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
func setContent(_ detailViewListContentView: UIView)
```

**macOS**

``` source
@MainActor
func setContent(_ detailViewListContentView: NSView)
```

## Parameters 

`detailViewListContentView`  

The `NSView` for the detail view content.

## See Also

### Setting view attributes

func setDetailViewListContent&lt;ListContent>(ListContent)

Sets the detail view for the list content.

func setDetailViewListContent&lt;ListContent>(() -> ListContent)

Sets the detail view for the list content from view builder closures.

func setShowManageButton(Bool)

A Boolean value the system uses to show or hide the default manage-participants button in the collaboration popover.

