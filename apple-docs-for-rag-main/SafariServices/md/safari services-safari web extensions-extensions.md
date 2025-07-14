

- Safari Services
-  Safari web extensions 

API Collection

# Safari web extensions

Create web extensions that work in Safari and other browsers.

## Overview

A Safari web extension adds custom functionality to Safari using JavaScript APIs and common file formats from extensions for Google Chrome, Mozilla Firefox, and Microsoft Edge browsers. While Safari app extensions are useful for sharing code between your native macOS app and Safari, you build Safari web extensions primarily on JavaScript, HTML, and CSS, and can repackage them to work in other browsers. You can also use Safari web extensions in Mac web apps.

Important

You implement a Safari web extension as a macOS, visionOS, or iOS app extension to provide a safe and secure distribution and usage model. You can distribute a Safari web extension with a Mac app, a visionOS app, an iOS app, or a Mac app created using Mac Catalyst. Use Xcode to package your extension for testing and distribution, and join the Apple Developer Program to distribute Safari web extensions. For more information, see Distributing your Safari web extension.

To get started with creating a Safari web extension, use one of the following options:

- Convert your existing extension into a Safari web extension, so you can use it in Safari in macOS, visionOS, and iOS and distribute it. Xcode includes a command-line tool to simplify this process.

- Build a new Safari web extension in Xcode using the built-in template. You can then repackage the extension files for deployment in other browsers.

- Temporarily install your web extension in Safari for testing without converting it or setting up an Xcode project. For more information, see Temporarily install a web extension folder in macOS Safari.

Learn more about the capabilities of web extensions and the APIs you use to build them in Mozilla’s Browser Extensions documentation.

Safari web extensions are available in macOS with Safari 14 and later, visionOS 1 and later, and iOS 15 and later. Safari web extensions are available in Mac web apps in macOS 15 and later.

## Topics

### New extensions

Creating a Safari web extension

Build a Safari web extension in Xcode.

Modernizing Safari Web Extensions

Learn about enhancements to Safari Web Extensions.

Developing a Safari Web Extension

Customize and enhance web pages by building a Safari web extension.

### Extension conversions

Converting a web extension for Safari

Convert your existing extension to a Safari web extension using Xcode’s command-line tool.

Converting a Safari app extension to a Safari web extension

Unify your web extensions and simplify development by sharing code with a Safari web extension.

### Extension updates

Updating a Safari web extension

Add new features and fix bugs in your Safari web extension using Xcode tools.

Managing Safari web extension permissions

Respect user privacy by setting appropriate permissions for your Safari web extension.

Previewing Metadata using Open Graph

Build a Safari Extension that displays metadata using Open Graph.

### Messaging

Messaging between the app and JavaScript in a Safari web extension

Communicate about events and share data between the containing app and JavaScript by using native messaging and app groups.

let SFExtensionMessageKey: String

A string the system uses as a key in a user info dictionary to identify a message.

let SFExtensionProfileKey: String

A string the system uses as a key in a user info dictionary to identify a profile identifier.

Messaging a Web Extension’s Native App

Communicate between your Safari web extension and its containing app.

Messaging between a webpage and your Safari web extension

Configure your extension to enable messaging from webpages, and then update your extension to handle messages.

### Blocking content

Blocking content with your Safari web extension

Build content blocking with declarative net request into your Safari web extension.

Adopting Declarative Content Blocking in Safari Web Extensions

Block web content with your web extension using the declarative net request API.

### Adding Web Inspector tools

Adding a web development tool to Safari Web Inspector

Expand the built-in Safari Web Inspector to include your custom tool, augmenting developers’ options for inspecting, testing, and debugging webpages.

Creating Safari Web Inspector extensions

Learn how to make custom Safari Web Inspector extensions.

### Extension improvements

Optimizing your web extension for Safari

Support Dark Mode, reduce memory and power usage, and ensure feature compatibility to improve your web extension experience in Safari and web apps.

Adopting New Safari Web Extension APIs

Improve your web extension in Safari with a non-persistent background page and new tab-override customization.

Syncing Safari web extensions across devices and platforms

Let users install your extension on one device and then use and manage the extension on all their other iOS and macOS devices.

Assessing your Safari web extension’s browser compatibility

Review your Safari web extension implementation plan, manifest keys, and JavaScript API usage for compatibility with other browsers.

Troubleshooting your Safari web extension

Use developer resources to investigate and resolve common problems with Safari web extensions.

### Installation and distribution

Running your Safari web extension

Install and update your extension in Safari as you make changes in development.

Distributing your Safari web extension

Get feedback on your extension from beta testers, then share your extension with customers in the App Store.

