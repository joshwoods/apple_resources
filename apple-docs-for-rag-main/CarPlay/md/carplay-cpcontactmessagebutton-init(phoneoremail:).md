

- CarPlay
- CPContactMessageButton
-  init(phoneOrEmail:) 

Initializer

# init(phoneOrEmail:)

Creates a contact message button with the provided contact information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(phoneOrEmail: String)
```

## Parameters 

`phoneOrEmail`  

A valid phone number or email address to use in Siri’s compose message flow.

## Return Value

A new contact message button.

## Discussion

The button displays a system image that communicates its function. CarPlay never displays the contact information you provide. Tapping the button activates Siri and launches the compose message flow using the phone number or email address you provide.

