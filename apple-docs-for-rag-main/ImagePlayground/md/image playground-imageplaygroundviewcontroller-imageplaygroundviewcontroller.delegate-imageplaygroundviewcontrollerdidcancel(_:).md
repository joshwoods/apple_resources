

- Image Playground
- ImagePlaygroundViewController
- ImagePlaygroundViewController.Delegate
-  imagePlaygroundViewControllerDidCancel(\_:) 

Instance Method

# imagePlaygroundViewControllerDidCancel(\_:)

Notifies the delegate that the person canceled the generation of the image.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
@MainActor @objc
optional func imagePlaygroundViewControllerDidCancel(_ imagePlaygroundViewController: ImagePlaygroundViewController)
```

## Parameters 

`imagePlaygroundViewController`  

The view controller that sent the notification.

## Discussion

Use this method to dismiss the specified ImagePlaygroundViewController from your app’s interface.

