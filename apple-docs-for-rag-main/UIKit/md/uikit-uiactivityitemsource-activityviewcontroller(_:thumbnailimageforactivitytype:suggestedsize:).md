

- UIKit
- UIActivityItemSource
-  activityViewController(\_:thumbnailImageForActivityType:suggestedSize:) 

Instance Method

# activityViewController(\_:thumbnailImageForActivityType:suggestedSize:)

For activities that support a preview image, returns a thumbnail preview image for the item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func activityViewController(
    _ activityViewController: UIActivityViewController,
    thumbnailImageForActivityType activityType: UIActivity.ActivityType?,
    suggestedSize size: CGSize
) -> UIImage?
```

## Parameters 

`activityViewController`  

The activity view controller object requesting information about the data item.

`activityType`  

The selected activity type.

`size`  

The suggested size for the thumbnail image, in points. You should provide an image using the appropriate scale for the screen. Images provided at the suggested size will result in the best experience.

## Return Value

The image to use as a preview for the item.

## See Also

### Providing information about the data items

func activityViewController(UIActivityViewController, subjectForActivityType: UIActivity.ActivityType?) -> String

For activities that support a subject field, returns the subject for the item.

func activityViewController(UIActivityViewController, dataTypeIdentifierForActivityType: UIActivity.ActivityType?) -> String

For items that are provided as data, returns the UTI for the item.

