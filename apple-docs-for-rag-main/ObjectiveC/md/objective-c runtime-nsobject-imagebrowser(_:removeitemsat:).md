

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:removeItemsAt:) 

Instance Method

# imageBrowser(\_:removeItemsAt:)

Signals that a remove operation should be applied to the specified items.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    removeItemsAt indexes: IndexSet!
)
```

## Parameters 

`aBrowser`  

An image browser view.

`indexes`  

The indexes of the items that should be removed.

## Discussion

This method is optional. It is invoked by the image browser after Image Kit determines that a remove operation should be applied. In response, the data source should update itself by removing the specified items.

