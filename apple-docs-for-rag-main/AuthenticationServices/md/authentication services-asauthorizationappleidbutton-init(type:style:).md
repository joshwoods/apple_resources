

- Authentication Services
- ASAuthorizationAppleIDButton
-  init(type:style:) 

Initializer

# init(type:style:)

Creates a new Sign In with Apple authorization button with the given type and style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    type: ASAuthorizationAppleIDButton.ButtonType,
    style: ASAuthorizationAppleIDButton.Style
)
```

## Parameters 

`type`  

The type of the button. Use one of the values from ASAuthorizationAppleIDButton.ButtonType.

`style`  

The style of the button. Use one of the values from ASAuthorizationAppleIDButton.Style.

## See Also

### Initializers

init(authorizationButtonType: ASAuthorizationAppleIDButton.ButtonType, authorizationButtonStyle: ASAuthorizationAppleIDButton.Style)

Creates a new Sign In with Apple authorization button with the given type and style.

