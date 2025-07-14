

- Social
- SLComposeViewController
-  setInitialText(\_:) 

Instance Method

# setInitialText(\_:)

Sets the initial text to be posted.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
func setInitialText(_ text: String!) -> Bool
```

## Parameters 

`text`  

The text to add to the post.

## Return Value

Returns a Boolean value that indicates whether the text was successfully set.

## Discussion

This method returns false if `text` does not fit in the currently available character space or if the view controller has already been presented to the user (and therefore cannot be changed). Character limits are dependent on the target service and are documented by the service provider. For links to documentation for the supported services, see Table 1 in SLRequest.

## See Also

### Specifying the Contents of the Post

func add(UIImage!) -> Bool

Adds an image to the post.

func add(URL!) -> Bool

Adds a URL to the post.

func removeAllImages() -> Bool

Removes all images from the post.

func removeAllURLs() -> Bool

Removes all URLs from the post.

