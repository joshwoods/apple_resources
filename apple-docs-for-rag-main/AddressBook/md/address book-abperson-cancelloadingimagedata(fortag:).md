

- Address Book
- ABPerson
-  cancelLoadingImageData(forTag:) 

Type Method

# cancelLoadingImageData(forTag:)

Cancels an asynchronous fetch of the images for a given tag.

macOS

``` source
class func cancelLoadingImageData(forTag tag: Int)
```

## Parameters 

`tag`  

The tag of the asynchronous fetch to be canceled.

## Discussion

The tag is returned from the previous call to the beginLoadingImageData(for:) method that started the asynchronous fetch.

## See Also

### Managing Images

func beginLoadingImageData(for: (any ABImageClient)!) -> Int

Starts an asynchronous fetch for image data in all locations

func imageData() -> Data!

Returns data that contains a picture of this person.

func setImageData(Data!) -> Bool

Sets the image for this person to the given data.

