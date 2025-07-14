

- Objective-C Runtime
- NSObject
-  numberOfItems(inImageBrowser:) 

Instance Method

# numberOfItems(inImageBrowser:)

Returns the number of records managed by the data source object.

macOS

``` source
func numberOfItems(inImageBrowser aBrowser: IKImageBrowserView!) -> Int
```

## Parameters 

`aBrowser`  

An image browser view.

## Return Value

The number of records managed by the image browser view.

## Discussion

Your data source must implement this method. An IKImageView object uses this method to determine how many cells it should create and display.

