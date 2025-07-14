

- Safari Release Notes
-  Safari 14.1 Release Notes 

Article

# Safari 14.1 Release Notes

Released April 26, 2021 — Version 14.1 (16611.1.21)

## Overview

Safari 14.1 ships with iOS & iPadOS 14.5 and macOS Big Sur 11.3.

### Authentication and Passwords

#### New Features

- Added support for Touch ID and Face ID via WebAuthentication to all WKWebViews. See Web Authentication for more information.

### CSS and Web Animations

#### New Features

- Added support for CSS individual transform properties: translate, rotate, and scale.

- Web Animations now support animating discrete properties and pseudo-elements, see Web Animations.

- Safari now supports flexbox gaps with `row-gap` and `column-gap`, see Gap Shorthand: the gap property.

### JavaScript and WebAssembly

#### New Features

- Added support for static instance class fields, private instance class fields, and static public class fields — public instance class fields were already supported. See Public and private instance fields proposal for more information.

- Added support for new ECMAScript Internationalization API features:

  - Added Intl.NumberFormat updates.

  - Added Intl.DisplayNames updates.

  - Added Intl.ListFormat updates.

  - Added Intl.Segmenter.

  - Added `Intl.DateTimeFormat` updates to dateStyle and timeStyle options on the Intl.DateTimeFormat API Specification, Intl.DateTimeFormat.prototype.formatRange, Add dayPeriod option, and Add fractionalSecondDigits option.

- Added support for WeakRefs and FinalizationRegistry.

- Added support for Arbitrary module namespace identifier names.

- Added support for WebAssembly atomic instructions in the Threading specification.

- Added support for WebAssembly BigInt integration.

- Added support for WebAssembly Sign-extension instructions.

### Media

#### New Features

- Added support for WebM files containing VP8 or VP9 video tracks and Vorbis audio tracks in macOS, see WebM Container Guidelines.

- Added support for MediaStream Recording to enable websites to record audio and video, see MediaStream Recording.

- Added support for getUserMedia from MediaStream and Capture API in WKWebView.

### Safari Web Extensions

#### New Features

- Added support for WebExtensions API to replace the new tab page.

- Added support for non-persistent background pages.

### Security and Privacy

#### New Features

- Improved Storage Access API interoperability and specification compliance, see Storage Access API.

- Added support for Private Click Measurement, enabling privacy-preserving ad attribution for web-to-web and app-to-web flows.

### WebKit Framework

#### New Features

- Added support for HTML `date`, `time`, and `datetime-local` input types in macOS, enabling date and time controls in forms. For more information, see Date state (type=date).

- Added support for Web Audio API, now unprefixed, compliant, and including Audio Worklets. This enables better compatibility for advanced audio processing, see Web Audio API for more information.

- Added support for Web Speech API that enables speech recognition and speech synthesis for websites.

- Improved mouse support in iPadOS and in apps built with Mac Catalyst, including scrolling events and hover/pointer media queries.

- Added support for Paint Timing, a Web API that measures how quickly a webpage is displayed. See Paint Timing 1 for more information.

## See Also

### Version 14

Safari 14 Release Notes

Released September 16, 2020 — Version 14 (16610.1.28)

