

- Security
- Password AutoFill
-  Enabling Password AutoFill on an HTML input element 

Article

# Enabling Password AutoFill on an HTML input element

Make sure a web view or webpage provides the correct AutoFill suggestions.

## Overview

To ensure your HTML input element displays the right AutoFill suggestion, set the `autocomplete` attribute for an `input` element.

Use the following `autocomplete` attribute values:

| Credential    | Autocomplete values |
|---------------|---------------------|
| User name     | `username`          |
| Password      | `current-password`  |
| New password  | `new-password`      |
| One-time code | `one-time-code`     |

Explicitly defining an input element’s autocomplete value lets you support login workflows that couldn’t otherwise be detected by Password AutoFill’s heuristics. For example, the heuristics assume the user name and password inputs are on the same page. If you have a multipage login form, explicitly setting the `username` and `current-password` types lets the user tap and fill those inputs, even if they’re on separate pages. Similarly, the heuristics assume that password and new password inputs always use secure text; therefore, if you want to let the user type their passwords in plain text, you’ll need to set the input’s text content type to either `current-password` or `new-password`.

By default, the system selects a keyboard based on the input element’s `autocomplete` value; however, you can mix the input element’s type and autocomplete values to explicitly define the desired keyboard. For example, if your site uses email addresses as user names, set the input view’s `autocomplete` attribute to `username`, and set the type property to `email`.

This example defines text fields for logging in:

```

```

When creating a new account or changing the password, use the `new-password` attribute value instead:

```

```

Additionally, you can autocomplete security codes from single-factor SMS login flows:

```

```

For more information on how to enable Password AutoFill behavior in iOS apps, see Enabling Password AutoFill on a text input view.

