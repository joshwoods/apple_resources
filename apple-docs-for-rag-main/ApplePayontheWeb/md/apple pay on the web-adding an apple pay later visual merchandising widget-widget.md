

- Apple Pay on the Web
-  Adding an Apple Pay Later visual merchandising widget 

Article

# Adding an Apple Pay Later visual merchandising widget

Configure and style Apple Pay Later visual merchandising widgets to match your website.

## Overview

Deprecated

Apple Pay Later is deprecated.

In iOS and iPadOS 16.4 and later, Apple Pay on the Web provides a variety of Apple Pay merchandising widget types that you can use on your website. You can specify the Apple Pay merchandising widget style, type, and localization using attributes that you supply to a JavaScript function that displays the widget.

### Add the Apple Pay JavaScript API to the page header

To display an Apple Pay Later visual merchandising widget, add the following script tag to your webpage’s `head` tag to load the Apple Pay JavaScript API:

```

```

The script tag contains the URL that loads the `apple-pay-sdk.js`, from the Apple Pay JS CDN. The script tag includes three additional attributes:

`crossorigin`  
An abbreviated version of `crossorigin=”anonymous”`, this attribute instructs the browser to connect to the Apple Pay JS CDN using anonymous credentials mode. This improves performance by allowing subsequent Apple Pay JS network requests to reuse the same HTTP/2 connection

`async`  
The attribute instructs the browser to immediately evaluate the script. This prevents `apple-pay-sdk.js` from blocking the page load, and initializes and loads the ApplePay JS libraries as soon as possible. Your app needs to wait for the callback function execution before interacting with the API.

`data-initial-token`  
This value is a JSON Web Token (JWT) that you need to obtain from the Developer Portal. See Certificates, Identifiers &amp; Profiles on the Developer Portal and follow the instructions for registering a merchant domain to generate the JWT.

Additionally, you need to ensure that your website allows a Content Security Policy for Apple Pay JS to function properly.

### Add a standard widget

To display the widget, add an `apple-pay-merchandising` tag to your webpage and set the amount, style, type, and locale parameters. For example, this call into the Apple Pay JavaScript library provides details necessary for rendering the widget localized to the US, and uses the default size and type:

```

```

There are several options for customizing the widget’s appearance:

| Attribute | Type | Description |
|----|----|----|
| `amount`  (required) | A string that represents the amount of the transaction as a decimal number, for example `“108”`. | The payment amount displayed in the widget, usually a product’s price. |
| `type` | `badge`, `plain`, `price`, or `checkout` | A string that describes the kind of Apple Pay Later visual merchandising widget. |
| `modal-type` | `learn-more` or `calculator` | A string that defines the contents of the modal that the visual merchandising widget displays. Use `learn-more` to display information about Apple Pay Later or `calculator` to display a breakdown of payments. |
| `locale` | An BCP 47 language code, such as `en-US`. | The language and region the widget uses for the Apple Pay Later visual merchandising widget. |
| `country-code`  (required) | A two-letter ISO-3166 country code. | The country or region of the merchant’s principal place of business. |
| `currency-code`  (required) | A three letter ISO-4217 currency code. | The currency in use at the merchant’s principal place of business |
| `theme` | `dark`, `light`, or `auto` | The appearance of the widget. Defaults to `auto` if no value is specified. |
| `debug` | `true` or `false` | The setting to use for testing purposes to force the widget to display on all devices and operating systems.  You need to remove this setting before deploying to production. |

### Determine sizing requirements

For sizing requirements for the Apple Pay Later visual merchandising widget, along with other design guidelines, see Apple Pay in the Human Interface Guidelines.

