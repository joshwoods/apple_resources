

- Bundle Resources
- Information Property List
-  ASWebAuthenticationSessionWebBrowserSupportCapabilities 

Property List Key

# ASWebAuthenticationSessionWebBrowserSupportCapabilities

A collection of keys that a browser app uses to declare its ability to handle authentication requests from other apps.

macOS 10.15+

## Details 

Type  

object

## Discussion

Add a dictionary for this key to your app’s Information Property List if your app is a web browser and it supports web authentication. In the dictionary, include the capability keys listed below to indicate your browser app’s capabilities. For more information, see Supporting Single Sign-On in a Web Browser App.

## Topics

### Capabilities

IsSupported

A Boolean that indicates whether the app acts as a browser that supports authentication sessions.

EphemeralBrowserSessionIsSupported

A Boolean that indicates whether the app supports ephemeral browsing when conducting authentication sessions.

CallbackURLMatchingIsSupported

A Boolean that indicates whether the app can handle callbacks to match authentication URLs.

AdditionalHeaderFieldsAreSupported

A Boolean that indicates whether the app supports additional header fields in requests.

## See Also

### Authentication

ASAccountAuthenticationModificationOptOutOfSecurityPromptsOnSignIn

A Boolean value that indicates the system shouldn’t show security recommendation prompts when users sign in using the app.

