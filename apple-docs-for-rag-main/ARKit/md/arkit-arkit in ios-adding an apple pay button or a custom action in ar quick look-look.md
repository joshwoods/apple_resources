

- ARKit
- ARKit in iOS
-  Adding an Apple Pay Button or a Custom Action in AR Quick Look 

Article

# Adding an Apple Pay Button or a Custom Action in AR Quick Look

Provide a banner that users can tap to make a purchase or perform a custom action in an AR experience.

## Overview

For AR experiences initiated through the web in iOS 13.3 or later, you can display an Apple Pay button so users can make purchases from your website.

Alternatively, you can provide text in the banner that users can tap to invoke a custom action in your website, like adding a previewed item to a shopping cart.

In addition, you can supply AR Quick Look with custom HTML that completely customizes the banner’s graphics.

To add an Apple Pay button or custom text or graphics in a banner, choose URL parameters to configure AR Quick Look for your website. Finally, detect and react to customer taps to the banner.

### Choose an Apple Pay Button Style

To select a style of Apple Pay button for your AR experience, append the `applePayButtonType` parameter to your website URL.

```
```

You can choose from the button options using the button type values shown here.

### Provide Custom Text

Instead of an Apple Pay button, you can supply text that AR Quick Look displays as a custom action button, as in the following image.

Append the `callToAction` URL parameter with the custom text as the value. The following example URL renders a banner with the text “Add to cart”:

```
```

Because URLs can’t contain spaces, be sure to URL-encode the custom text before appending it as a URL parameter. If your website supports multiple languages, localize the custom text before URL-encoding it for the URL parameter list.

### Define the Item

When you add an Apple Pay button or a custom action button to AR Quick Look, set the description of the previewed items using the `checkoutTitle`, `checkoutSubtitle`, and `price` URL parameters. AR Quick Look displays the subtitle and price separated by a comma below the title.

If AR Quick Look can’t fit the subtitle and price on one line, it truncates the subtitle with an ellipsis. The following example URL renders the banner.

```
```

If your website supports multiple languages, localize the item title, subtitle, and price before URL-encoding them for the URL parameter list.

### Display a Custom Banner

To take full control of the banner’s graphics, supply a custom HTML file through the `custom` URL parameter. The following example URL renders a banner from a custom file named `comingSoonBanner`.

```
```

This example URL creates the AR experience illustrated below.

If you use the `custom` URL parameter, the value must be an absolute URL. To comply with AR Quick Look’s security standards, ensure the server sends the HTML resource over HTTPS.

Important

AR Quick Look displays the contents of the HTML only. If you embed actions such as links or events, AR Quick Look ignores them.

### Define the Custom Banner’s Height

When you display a custom banner, you can set the banner height using the `customHeight` URL parameter.

Supply a value of `small`, `medium`, or `large` to set the banner height to 81, 121, or 161 points, respectively. For example:

```
```

AR Quick Look automatically scales the width of the banner to the size and orientation of the device on which it displays. The maximum width of the custom banner is 450 points. If you omit the `customHeight` URL parameter, AR Quick Look uses the default value, `small`.

### Detect a Tap

When the user taps the Apple Pay button or custom action button, WebKit sends a DOM message to the `` element of your code that references the 3D asset.

```
```

To be notified of the tap, define a JavaScript listener for the `message` event on your anchor.

```
```

When WebKit invokes your listener, check the `data` property. A value of `_apple_ar_quicklook_button_tapped` confirms the user tapped the banner in AR Quick Look.

```
```

The `message` event follows normal DOM processing rules. Rather than adding a listener for a specific anchor, you can add a listener at the document root for all AR links, and use the `event.target` to determine which anchor the user invoked.

### React to a Tap

Define the actions your website takes in response to a user tap in your event listener. When the user taps the custom action button, you might add the previewed item to a shopping cart or take the user to a checkout page, depending on the banner’s text and custom action.

If your banner displays an Apple Pay button, bring up the Apple Pay prompt using Apple Pay JS API.

If your banner displays an Apple Messages for Business button, send the user to Messages using your company’s custom Apple Messages for Business URL. For more infomation, see Starting a Chat from a URL.

## See Also

### AR Quick Look

Previewing a Model with AR Quick Look

Display a model or scene that the user can move, scale, and share with others.

Adding Visual Effects in AR Quick Look and RealityKit

Balance the appearance and performance of your AR experiences with modeling strategies.

class ARQuickLookPreviewItem

An object for customizing the AR Quick Look experience.

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

Specifying a lighting environment in AR Quick Look

Add metadata to your USDZ file to specify its lighting characteristics.

