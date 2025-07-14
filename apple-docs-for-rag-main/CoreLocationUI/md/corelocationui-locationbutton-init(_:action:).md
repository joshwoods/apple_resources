

- CoreLocationUI
- LocationButton
-  init(\_:action:) 

Initializer

# init(\_:action:)

Creates a location button with the specified title and action.

CoreLocationUISwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
nonisolated
init(
    _ title: LocationButton.Title? = .currentLocation,
    action: @escaping () -> Void
)
```

## Parameters 

`title`  

The text that the button displays. For possible values, see LocationButton.Title.

`action`  

The action that initiates every time the user taps the button.

## See Also

### Creating a location button

struct Title

Constants that specify the text of a button title.

