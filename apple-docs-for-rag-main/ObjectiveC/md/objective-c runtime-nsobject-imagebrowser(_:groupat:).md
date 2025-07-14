

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:groupAt:) 

Instance Method

# imageBrowser(\_:groupAt:)

Returns the group at the specified index.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    groupAt index: Int
) -> [AnyHashable : Any]!
```

## Parameters 

`aBrowser`  

An image browser view.

`index`  

The index of the group you want to retrieve.

## Return Value

A dictionary that defines the group. The keys in this dictionary can be any of the following constants: IKImageBrowserGroupStyleKey, IKImageBrowserGroupBackgroundColorKey, IKImageBrowserGroupTitleKey, and IKImageBrowserGroupRangeKey. For more information on these constants, see IKImageBrowserView.

## Discussion

This method is optional.

