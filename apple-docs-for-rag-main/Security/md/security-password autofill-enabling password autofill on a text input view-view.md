

- Security
- Password AutoFill
-  Enabling Password AutoFill on a text input view 

Article

# Enabling Password AutoFill on a text input view

Make sure a text input view displays the correct AutoFill suggestions.

## Overview

To ensure your text input view displays the right AutoFill suggestions, set the textContentType property on any relevant input views.

Use the following UITextContentType values:

| Credential | `UITextContentType` value |
|----|----|
| User name | username |
| Password | password |
| New password | newPassword |
| One-time code | oneTimeCode |

Explicitly defining a view’s text content type improves the performance of Password AutoFill’s heuristics and lets you support login workflows that couldn’t otherwise be detected by these heuristics. For example, the heuristics assume the user name and password inputs are on the same page. If you have a multipage login form, explicitly setting the username and password types lets the user tap and fill those inputs, even if they’re on separate pages.

Important

tvOS apps can also support Password AutoFill using the same content-type settings. The AutoFill QuickType bar appears above the keyboard when entering passwords with an iOS device using the Control Center keyboard, the Remote app, or the Continuity Keyboard. Focus is also advanced to the login button when the login fields are populated.

By default, the system selects a keyboard based on the input view’s textContentType property; however, you can mix the input view’s text content type and keyboard type to explicitly define the desired keyboard. For example, if your site uses email addresses as user names, set the input view’s textContentType property to username, and set the keyboardType property to UIKeyboardType.emailAddress.

Note

Leverage the system keyboard rather than implementing a keyboard directly in your app’s view hierarchy.

This example defines text fields for logging in:

```
userTextField.textContentType = .username
userTextField.keyboardType = .emailAddress
passwordTextField.textContentType = .password
```

When creating a new account or changing the password, use the newPassword text content type instead:

```
newPasswordTextField.textContentType = .newPassword
confirmPasswordTextField.textContentType = .newPassword
```

Additionally, you can autocomplete security codes from single-factor SMS login flows:

```
singleFactorCodeTextField.textContentType = .oneTimeCode
```

iOS supports Password AutoFill on UITextField, UITextView, and any custom view that adopts the UITextInput protocol.

Warning

If you use a custom input view for a security code input text field, iOS can’t display the necessary AutoFill UI.

For more information on how to enable Password AutoFill behavior in web apps, see Enabling Password AutoFill on an HTML input element.

