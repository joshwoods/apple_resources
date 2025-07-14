

- UIKit
- UIActivityItemSource
-  activityViewController(\_:dataTypeIdentifierForActivityType:) 

Instance Method

# activityViewController(\_:dataTypeIdentifierForActivityType:)

For items that are provided as data, returns the UTI for the item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func activityViewController(
    _ activityViewController: UIActivityViewController,
    dataTypeIdentifierForActivityType activityType: UIActivity.ActivityType?
) -> String
```

## Parameters 

`activityViewController`  

The activity view controller object requesting information about the data item.

`activityType`  

The selected activity type; may be `nil`.

## Return Value

The UTI for the item.

## Discussion

Providing the UTI allows services to handle specific data types in appropriate ways, such as an email service formatting an image to display in-line. If you provide items as NSData objects, implement this method to allow those services to better handle your data.

To ensure that Mail can handle an attachment that uses your exported UTI, include the UTExportedTypeDeclarations key in your app’s `Info.plist` file, describing the UTI and providing the MIME type for it. The following example shows how `public.jpeg` might be defined as an exported type (only the required keys are shown):

```
UTExportedTypeDeclarations

                UTTypeIdentifier
                public.jpeg
                UTTypeConformsTo

                    public.image
                    public.data

                UTTypeTagSpecification

                    com.apple.ostype
                    JPEG
                    public.filename-extension

                        jpeg
                        jpg

                    public.mime-type
                    image/jpeg

```

## See Also

### Providing information about the data items

func activityViewController(UIActivityViewController, subjectForActivityType: UIActivity.ActivityType?) -> String

For activities that support a subject field, returns the subject for the item.

func activityViewController(UIActivityViewController, thumbnailImageForActivityType: UIActivity.ActivityType?, suggestedSize: CGSize) -> UIImage?

For activities that support a preview image, returns a thumbnail preview image for the item.

