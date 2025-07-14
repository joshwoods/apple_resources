

- UIKit
- UICloudSharingControllerDelegate
-  itemThumbnailData(for:) 

Instance Method

# itemThumbnailData(for:)

Asks the delegate for the thumbnail image data to display on the invitation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func itemThumbnailData(for csc: UICloudSharingController) -> Data?
```

## Discussion

Implement this method to return image data representing the shared recording. Returning `nil` tells the UICloudSharingController instance to display the generic image. Not implementing this method is the same as returning `nil`.

itemThumbnailData(for:) is called only when creating a new share. For an existing share, the thumbnail image is retrieved from the share using the CKShareThumbnailImageDataKey key.

The following code shows an example of retrieving the image data from a data set stored in an asset catalog found in the main bundle.

```
- (nullable NSData *)itemThumbnailDataForCloudSharingController:(UICloudSharingController *)csc
{  
  NSDataAsset *icon = [[NSDataAsset alloc] initWithName:@"thumbnail"];
  return [icon data];
}
```

## See Also

### Configuring the view controller

func itemTitle(for: UICloudSharingController) -> String?

Asks the delegate for the title to display on the invitation screen.

**Required**

func itemType(for: UICloudSharingController) -> String?

Asks the delegate for the Uniform Type Identifier (UTI) of the item.

