

- UIKit
- UICloudSharingControllerDelegate
-  itemType(for:) 

Instance Method

# itemType(for:)

Asks the delegate for the Uniform Type Identifier (UTI) of the item.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func itemType(for csc: UICloudSharingController) -> String?
```

## Discussion

UICloudSharingController uses the UTI to determine if the shared item is a special type. This allows text presented by the controller to refer to the item using descriptive wording. For example, if the shared item is a presentation and `kUTTypePresentation` is returned, the screens refer to the shared item as a *presentation*. Likewise, if the shared item is a document and `kUTTypeContent` is returned, the screens refer to the item as a *document*. And when `kUTTypeSpreadsheet` is returned, the screens refer to the item as a *spreadsheet*.

For types unique to your app, return `nil` or do not implement this method.

- Swift
- Objective-C

```
func itemType(for csc: UICloudSharingController) -> String? {
  return kUTTypePNG as String // Add "import MobileCoreServices" to use UTI constants.
}
```

```
- (nullable NSString *)itemTypeForCloudSharingController:(UICloudSharingController *)csc
{
  return (NSString*)kUTTypePNG; // Add #import  to use UTI constants.
}
```

## See Also

### Configuring the view controller

func itemTitle(for: UICloudSharingController) -> String?

Asks the delegate for the title to display on the invitation screen.

**Required**

func itemThumbnailData(for: UICloudSharingController) -> Data?

Asks the delegate for the thumbnail image data to display on the invitation.

