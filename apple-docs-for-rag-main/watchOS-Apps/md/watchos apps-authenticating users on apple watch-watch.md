

- watchOS apps
-  Authenticating users on Apple Watch 

Article

# Authenticating users on Apple Watch

Create an account sign-up and sign-in strategy for your app.

## Overview

Users can launch an independent watchOS app as soon as it downloads, even if they don’t have their iPhone. As a result, users must be able to set up the application directly on Apple Watch. If your app requires an account, users must be able to create it and sign in on the watch.

You have the following options for syncing or saving user data:

- Create an app that doesn’t require user accounts. Design your app so that it provides a full set of features without user accounts, or use CloudKit to sync and store your user’s data. Apps can access CloudKit data based on the user’s Apple ID without in-app sign-in. watchOS 6 and later also supports CloudKit subscriptions and notifications to let your app respond to changes from other devices.

- Authenticate users with Sign In with Apple. This feature authenticates users based on their Apple ID. For more information, see WKInterfaceAuthorizationAppleIDButton and Authentication Services.

- Create custom sign-in and sign-up forms.

If you choose to create custom forms, watchOS 6 provides tools designed to fit the small screen size and to streamline data entry on Apple Watch.

### Simplify account creation and sign-in

Create your sign-in and sign-up forms using text fields. In SwiftUI, use the TextField and SecureField structures. In the storyboard, use the WKInterfaceTextField class.

To streamline data entry, perform the following steps:

1.  Set the text field’s content type. The text field’s content type modifies how the text input controller and Apple Continuity Keyboard behave. For SwiftUI, set the content type by calling the text field’s textContentType(_:) method. For the storyboard, set the content type using the Attributes inspector.

2.  Provide a placeholder that describes the text field’s expected content. Effective placeholders help you get the most out of Apple Watch’s smaller screen. For SwiftUI, when instantiating the text field, the `title` property sets the placeholder. For the storyboard, set the placeholder using the Attributes inspector. Note that the system truncates placeholders if the text is too long, so keep your placeholders short.

3.  Set up your app’s associated domains. If you have a website where users can sign in with the same username and password, associate the website’s domain with your app. An associated domain tells the Apple Continuity Keyboard to provide autofill suggestions for usernames and passwords from that domain. To learn how to set up your app’s associated domains, see Supporting associated domains.

### Support password autofill

To support password autofill on Apple Watch, set the following WKTextContentType values.

| Credential | Content Type |
|----|----|
| User Name | username |
| Password | password |
| New Password | newPassword |
| One-Time Code | oneTimeCode |

For TextField and SecureField, set the content type by calling the textContentType(_:) method.

```
```

For WKInterfaceTextField, assign these values in Xcode by setting the Content Type attribute in the Attributes inspector.

watchOS provides an autofill suggestion for oneTimeCode fields after receiving an SMS message that contains a one-time code.

If you place a username or emailAddress text field on the same screen as a password text field, the Apple Continuity Keyboard attempts to fill both fields. Similarly, if you put two newPassword fields on the same screen, the keyboard automatically fills both when the user selects the suggested password.

For more information, see Password AutoFill.

## See Also

### App experience

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

Creating independent watchOS apps

Set up a watchOS app that installs and runs without a companion iOS app.

Keeping your watchOS content up to date

Ensure that your app’s content is relevant and up to date.

Updating watchOS apps with timelines

Seamlessly schedule updates to your user interface, even while it’s inactive.

Responding to the Action button on Apple Watch Ultra

Use App Intents to register actions for your app.

Enabling the double-tap gesture on Apple Watch

Customize your app’s response to the double-tap gesture on Apple Watch.

