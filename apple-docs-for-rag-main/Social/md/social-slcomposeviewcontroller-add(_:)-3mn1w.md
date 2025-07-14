

- Social
- SLComposeViewController
-  add(\_:) 

Instance Method

# add(\_:)

Adds a URL to the post.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
func add(_ url: URL!) -> Bool
```

## Parameters 

`url`  

The URL to add to the post.

## Return Value

Returns a Boolean value that indicates whether the URL was successfully added.

## Discussion

This method returns false if `url` does not fit in the currently available character space or if the view controller has already been presented to the user (and therefore cannot be changed). Character limits are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Specifying the Contents of the Post

func setInitialText(String!) -> Bool

Sets the initial text to be posted.

func add(UIImage!) -> Bool

Adds an image to the post.

func removeAllImages() -> Bool

Removes all images from the post.

func removeAllURLs() -> Bool

Removes all URLs from the post.

