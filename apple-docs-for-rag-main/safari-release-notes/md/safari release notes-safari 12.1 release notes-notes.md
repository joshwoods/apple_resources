

- Safari Release Notes
-  Safari 12.1 Release Notes 

Article

# Safari 12.1 Release Notes

Released March 25, 2019 — Version 12.1 (14607.1.40)

## Overview

Safari 12.1 ships with iOS 12.2 and macOS 10.14.4. It’s also available for macOS 10.13.6 and 10.12.6.

New features of Safari 12.1 include:

- **Dark Mode for the Web.** The ability to enable color scheme customizations for websites while in Dark Mode.

- **Intelligent Tracking Prevention.** New permission requirements for third-party cookies and new limits for long-term tracking.

### General

#### New Features

- Updated the push notification prompt for Safari on macOS to require a user gesture.

#### Resolved Issues

- Updated the behavior of websites saved to the home screen on iOS to pause in the background instead of relaunching each time.

### Authentication and Passwords

#### New Features

- Updated Password AutoFill to sign in automatically to websites after filling in the credentials.

### Security and Privacy

#### New Features

- Added warnings displayed to the user when loading insecure pages in both Safari and in SFSafariViewController.

- Added Motion & Orientation settings on iOS to enable the DeviceMotionEvent and DeviceOrientationEvent events.

- Removed support for the expired Do Not Track standard to prevent potential use as a fingerprinting variable.

- Updated the link behavior for `"target=_blank"` to include `rel="noopener" implicitly`.

### Intelligent Tracking Prevention

#### New Features

- Removed support for partitioned cookies for domains with cross-site tracking capabilities. The Storage Access API now provides third-party access to cookies.

- Improved Intelligent Tracking Prevention to limit long-term tracking based on client-side first-party cookies and to verify partitioned cache entries.

### Web API

#### New Features

- Added a `supported-color-schemes` meta tag to indicate a website supports `light` and `dark` color schemes.

- Added support for the Intersection Observer API, which detects the intersection of visible elements relative to other elements. Elements include the viewport of the top-level document.

- Added support for the Web Share API to invoke the native share dialog provided by the system.

- Added support for ``.

- Added support for the `` element.

### Payment Request API

#### New Features

- Added support for granular errors.

- Added support in Wallet & Apple Pay preferences for using the default contact information for the shipping address, email, and phone. On iOS, set preferences in the Transaction Defaults category in Settings \> Wallet & Apple Pay. On Mac, set preferences in System Preferences \> Wallet & Apple Pay \> Contacts and Shipping.

- Added support for the default addresses and contacts configured in the Contacts and Shipping in the Wallet system preferences on iOS and macOS.

- Added support for special fields for Japan including `phoneticName`, subLocality, and subAdministrativeArea.

### CSS and Text

#### New Features

- Added support for the CSS media queries `prefers-color-scheme: light` and `prefers-color-scheme: dark`.

- Added support for CSS rules to customize text decorations like underlines and dashed underlines.

- Added support for new `rgb()` color functions from the CSS Color 4 specification.

### Media

#### New Features

- Added support for H.264 simulcast and VP8 in WebRTC to improve support for multi-party video conferencing.

- Enabled cross-browser Encrypted Media Extensions (EME) by adding APIs without the `webkit` prefix.

### Safari App Extension API

#### New Features

- Added getAllWindows(completionHandler:) and getAllTabs(completionHandler:) for iterating over all open windows and tabs.

- Added getContainingTab(completionHandler:) and getContainingWindow(completionHandler:) access to the containing tab and window objects.

- Added a `close` method to SFSafariWindow and SFSafariTab for closing windows and tabs.

- Added navigate(to:) for changing the URL of a tab.

- Added getScreenshotOfVisibleArea(completionHandler:) for taking a screenshot of the visible contents of a page.

- Added showPopover() and dismissPopover() for showing and dismissing extension popovers.

- Added getBaseURI(completionHandler:) for retrieving the base URI in the app extension process.

- Improved support for navigating backwards and forwards.

### Web Inspector and Tools

#### New Features

- Added support for multiple selection of DOM tree nodes and of entries in the Cookies table.

- Improved styles editing with multiple selection support.

- Updated Timelines to include media events.

## See Also

### Version 12

Safari 12 Release Notes

Released September 17, 2018 — Version 12 (14606.1.36)

