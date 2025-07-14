

- Address Book
- ABPerson
-  imageData() 

Instance Method

# imageData()

Returns data that contains a picture of this person.

macOS

``` source
func imageData() -> Data!
```

## Return Value

Data containing a picture of this person

## Discussion

This method searches only the local file system and operates synchronously. To perform an asynchronous search or to search over a network, use beginLoadingImageData(for:).

The returned data is in a QuickTime-compatible format. To create an image from it, use the `NSImage` method init(data:).

## See Also

### Managing Images

class func cancelLoadingImageData(forTag: Int)

Cancels an asynchronous fetch of the images for a given tag.

func beginLoadingImageData(for: (any ABImageClient)!) -> Int

Starts an asynchronous fetch for image data in all locations

func setImageData(Data!) -> Bool

Sets the image for this person to the given data.

