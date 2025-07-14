

- Safari Release Notes
-  Safari 16.1 Release Notes 

Article

# Safari 16.1 Release Notes

Released October 24, 2022 — Version 16.1 (18614.2.9)

### Overview

Safari 16.1 is available for macOS Big Sur, macOS Monterey, macOS Ventura, iPadOS 16.1 and iOS 16.1.

### Accessibility

#### Resolved Issue

- Fixed `display:contents` buttons failing to expose their accessible name.

### Authentication

#### New Feature

- Added support for passkeys on macOS Big Sur, macOS Monterey, macOS Ventura, and iPadOS 16.1. See Supporting passkeys.

### CSS

#### Resolved Issues

- Fixed dynamic viewport height units (`dvh`) not matching the actual viewport height.

- Fixed scroll-snap properties set on `` to stop propagating to the viewport.

- Fixed logical viewport units to properly resolve for `font-size`.

- Fixed containing blocks with a non-visible overflow incorrectly clipping `position: fixed` descendants.

- Fixed table user-agent styles to use `box-sizing: border-box`.

- Fixed `` elements with `contain: size`.

- Fixed handling layout and paint containment.

- Fixed handling `font-variant: normal` and `font-variant: none` shorthands to reset `font-variant-numeric` and `font-variant-alternates`.

- Fixed small caps handling to prevent synthesized small caps if any character in the font supports small caps.

### Forms

#### Resolved Issues

- Fixed the ignored CSS `color` property on `` elements.

- Fixed `` with `appearance: textfield` to hide icons.

- Fixed applying the readonly attribute to the correct `` types and `` element.

- Fixed the content width for `` to not include decorations.

- Fixed input type state changes to correctly handle missing or empty string value attributes.

- Fixed `form.submit()` to submit a single form to multiple frames concurrently.

- Fixed cloning a `` to not set the initial selection at the end of the text content.

- Fixed not firing a select event when setting a selection range results in no change to the selection.

### Media

#### New Features

- Added support for non-animated AVIF on macOS Ventura, and iPadOS 16.

- Added support for AVIF animated image sequences on macOS Ventura, iPadOS 16, and iOS 16.

#### Resolved Issues

- Fixed some AVIF images not rendering because of their container format.

### Privacy

New Features

- Added support for web-to-App Store advertising with SKAdNetwork.

### Rendering

#### Resolved Issues

- Stopped propagating background on `` with any containment.

### Security

#### Resolved Issues

- Fixed COOP `same-origin` breaking forms after a back navigation.

- Fixed `script-src-elem` CSP in workers.

### Web API

#### New Features

- Added Web Push Notifications support on macOS Ventura.

- Added support for capturing a specific window with `getDisplayMedia()` on macOS Ventura.

- Added support for Scroll to Text Fragment.

#### Resolved Issues

- Fixed focus interactions between the shadow DOM and the `` element to align with specifications.

### Web Driver

#### New Features

- Added support for Wheel input source and actions.

### Web Inspector

#### New Features

- Added support for the color picker to pick a color from any pixel on the screen.

## See Also

### Version 16

Safari 16.6 Release Notes

Released July 24, 2023 — Version 16.6 (18615.3.12)

Safari 16.5 Release Notes

Released May 18, 2023 — Version 16.5 (18615.2.9)

Safari 16.4 Release Notes

Released March 27, 2023 — Version 16.4 (18615.1.26)

Safari 16.3 Release Notes

Released January 23, 2023 — Version 16.3 (18614.4.6)

Safari 16.2 Release Notes

Released December 13, 2022 — Version 16.2 (18614.3.7)

Safari 16 Release Notes

Released September 12, 2022 — Version 16 (18614.1.25)

