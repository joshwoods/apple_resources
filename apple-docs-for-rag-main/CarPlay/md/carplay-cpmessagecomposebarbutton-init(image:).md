

- CarPlay
- CPMessageComposeBarButton
-  init(image:) 

Initializer

# init(image:)

Creates a message compose button that displays a custom image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(image: UIImage)
```

## Parameters 

`image`  

The image to display on the button.

## Return Value

A message compose button with the custom image.

## Discussion

Note

This button type does not use a handler. Instead, tapping this button activates Siri and initiates the compose message flow.

## See Also

### Creating a Message Compose Bar Button

init()

Creates a message compose button with a system-provided image.

