

- Image Playground
- ImagePlaygroundViewController
- ImagePlaygroundViewController.Delegate
-  imagePlaygroundViewController(\_:didCreateImageAt:) 

Instance Method

# imagePlaygroundViewController(\_:didCreateImageAt:)

Returns the generated image to the delegate.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
@MainActor @objc
func imagePlaygroundViewController(
    _ imagePlaygroundViewController: ImagePlaygroundViewController,
    didCreateImageAt imageURL: URL
)
```

**Required**

## Parameters 

`imagePlaygroundViewController`  

The view controller that sent the notification.

`imageURL`  

The location of the generated image. The file will live inside a temporary folder of your app sandbox. The app should move it to a permanent location or clean it up when it has finished using the file.

## Discussion

Use this method to retrieve the image at the specified location. After you finish retrieving the image, dismiss the ImagePlaygroundViewController from your app’s interface.

