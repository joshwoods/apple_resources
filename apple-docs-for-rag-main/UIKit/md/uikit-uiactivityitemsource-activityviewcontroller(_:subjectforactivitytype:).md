

- UIKit
- UIActivityItemSource
-  activityViewController(\_:subjectForActivityType:) 

Instance Method

# activityViewController(\_:subjectForActivityType:)

For activities that support a subject field, returns the subject for the item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func activityViewController(
    _ activityViewController: UIActivityViewController,
    subjectForActivityType activityType: UIActivity.ActivityType?
) -> String
```

## Parameters 

`activityViewController`  

The activity view controller object requesting information about the data item.

`activityType`  

The selected activity type; may be `nil`.

## Return Value

A string to use as the contents of the subject field.

## Discussion

When posting an item the service may provide for a separate subject field and data field, such as an email message. Implement this method if you wish to provide a subject field for services that support one.

## See Also

### Providing information about the data items

func activityViewController(UIActivityViewController, dataTypeIdentifierForActivityType: UIActivity.ActivityType?) -> String

For items that are provided as data, returns the UTI for the item.

func activityViewController(UIActivityViewController, thumbnailImageForActivityType: UIActivity.ActivityType?, suggestedSize: CGSize) -> UIImage?

For activities that support a preview image, returns a thumbnail preview image for the item.

