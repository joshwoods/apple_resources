

- Social
- SLComposeViewController
-  removeAllURLs() 

Instance Method

# removeAllURLs()

Removes all URLs from the post.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
func removeAllURLs() -> Bool
```

## Return Value

Returns a Boolean value that indicates whether the URLs were successfully removed.

## Discussion

If the view controller has already been presented to the user when removeAllURLs() is called, the method returns false and the URLS are not removed.

## See Also

### Specifying the Contents of the Post

func setInitialText(String!) -> Bool

Sets the initial text to be posted.

func add(UIImage!) -> Bool

Adds an image to the post.

func add(URL!) -> Bool

Adds a URL to the post.

func removeAllImages() -> Bool

Removes all images from the post.

