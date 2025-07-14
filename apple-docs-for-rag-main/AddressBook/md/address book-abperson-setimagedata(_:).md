

- Address Book
- ABPerson
-  setImageData(\_:) 

Instance Method

# setImageData(\_:)

Sets the image for this person to the given data.

macOS

``` source
func setImageData(_ data: Data!) -> Bool
```

## Parameters 

`data`  

The image to be set.

## Discussion

The `data` argument must be in a QuickTime-compatible format. Pass `nil` to specify that there is no image for this person.

## See Also

### Managing Images

class func cancelLoadingImageData(forTag: Int)

Cancels an asynchronous fetch of the images for a given tag.

func beginLoadingImageData(for: (any ABImageClient)!) -> Int

Starts an asynchronous fetch for image data in all locations

func imageData() -> Data!

Returns data that contains a picture of this person.

