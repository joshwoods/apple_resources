

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:itemAt:) 

Instance Method

# imageBrowser(\_:itemAt:)

Returns an object for the item in an image browser view that corresponds to the specified index.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    itemAt index: Int
) -> Any!
```

## Parameters 

`aBrowser`  

An image browser view.

`index`  

The index of the item you want to retrieve.

## Return Value

An `IKImageBrowserItem` object.

## Discussion

Your data source must implement this method. The returned object must implement the required methods of the IKImageBrowserItem protocol.

