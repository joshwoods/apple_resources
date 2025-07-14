

- Address Book
- ABPerson
-  beginLoadingImageData(for:) 

Instance Method

# beginLoadingImageData(for:)

Starts an asynchronous fetch for image data in all locations

macOS

``` source
func beginLoadingImageData(for client: (any ABImageClient)!) -> Int
```

## Parameters 

`client`  

The object to be notified when the image finishes loading.

## Return Value

A nonzero tag for tracking. This tag is used by the cancelLoadingImageData(forTag:) method to cancel a fetch operation.

## Discussion

The `client` object should conform to the `ABImageClient` protocol. A consumeImageData(_:forTag:) message is sent to `client` when the fetch is done. Use the cancelLoadingImageData(forTag:) method if you need to cancel an asynchronous fetch.

## See Also

### Managing Images

class func cancelLoadingImageData(forTag: Int)

Cancels an asynchronous fetch of the images for a given tag.

func imageData() -> Data!

Returns data that contains a picture of this person.

func setImageData(Data!) -> Bool

Sets the image for this person to the given data.

