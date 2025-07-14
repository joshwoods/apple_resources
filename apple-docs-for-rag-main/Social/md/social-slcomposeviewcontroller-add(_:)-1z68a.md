

- Social
- SLComposeViewController
-  add(\_:) 

Instance Method

# add(\_:)

Adds an image to the post.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
func add(_ image: UIImage!) -> Bool
```

## Parameters 

`image`  

The image to add to the post.

## Return Value

Returns a Boolean value that indicates whether the image was successfully added.

## Discussion

This method returns false if `image` does not fit in the currently available space, or if the view controller has already been presented to the user (and therefore cannot be changed). For the accepted `UIImage` formats, see Figure 2. Image size limits are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Specifying the Contents of the Post

func setInitialText(String!) -> Bool

Sets the initial text to be posted.

func add(URL!) -> Bool

Adds a URL to the post.

func removeAllImages() -> Bool

Removes all images from the post.

func removeAllURLs() -> Bool

Removes all URLs from the post.

