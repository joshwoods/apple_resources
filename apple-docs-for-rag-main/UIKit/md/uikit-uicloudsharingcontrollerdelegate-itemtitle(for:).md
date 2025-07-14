

- UIKit
- UICloudSharingControllerDelegate
-  itemTitle(for:) 

Instance Method

# itemTitle(for:)

Asks the delegate for the title to display on the invitation screen.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func itemTitle(for csc: UICloudSharingController) -> String?
```

**Required**

## Discussion

Implement this method to provide a meaningful title to the UICloudSharingController invitation screen.

itemTitle(for:) is called only when creating a new share. For an existing share, the title is retrieved from the share using the CKShareTitleKey key, which is set when a new share is saved.

- Swift
- Objective-C

```
func itemTitle(for csc: UICloudSharingController) -> String? {
  return "Untitled"
}
```

```
- (nullable NSString *)itemTitleForCloudSharingController:(UICloudSharingController *)csc
{
  return @"Untitled";
}
```

## See Also

### Configuring the view controller

func itemType(for: UICloudSharingController) -> String?

Asks the delegate for the Uniform Type Identifier (UTI) of the item.

func itemThumbnailData(for: UICloudSharingController) -> Data?

Asks the delegate for the thumbnail image data to display on the invitation.

