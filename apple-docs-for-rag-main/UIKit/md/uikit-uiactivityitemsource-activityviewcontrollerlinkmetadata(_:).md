

- UIKit
- UIActivityItemSource
-  activityViewControllerLinkMetadata(\_:) 

Instance Method

# activityViewControllerLinkMetadata(\_:)

Returns metadata to display in the preview header of the share sheet.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
optional func activityViewControllerLinkMetadata(_ activityViewController: UIActivityViewController) -> LPLinkMetadata?
```

## Parameters 

`activityViewController`  

The UIActivityViewController object requesting information about the item that the user wants to share.

## Return Value

The LPLinkMetadata object that contains the metadata about a URL, including its title, icon, images, and video.

## Discussion

Using the Link Presentation framework, you can display rich previews of web links inside your app. For instance, if your app already has a database of links, with titles and images that weren’t fetched by LPMetadataProvider, you don’t have to fetch new metadata from the internet. Use this method instead and avoid downloading it again.

In your implementation, create an LPLinkMetadata object, and fill in at least the originalURL and url fields, plus whatever additional information you have.

```
func activityViewControllerLinkMetadata(_: UIActivityViewController) -> LPLinkMetadata? {
    let metadata = LPLinkMetadata()
    metadata.originalURL = URL(string: "https://www.example.com/apple-pie")
    metadata.url = metadata.originalURL
    metadata.title = "The Greatest Apple Pie In The World"
    metadata.imageProvider = NSItemProvider.init(contentsOf:
        Bundle.main.url(forResource: "apple-pie", withExtension: "jpg"))
    return metadata
}
```

To learn more about presenting rich links and accelerating the share sheet, see Link Presentation and LPMetadataProvider, or watch the WWDC 2019 session 262: Embedding and Sharing Visually Rich Links.

