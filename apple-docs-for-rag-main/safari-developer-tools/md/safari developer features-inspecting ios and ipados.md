

- Safari Developer Features
-  Inspecting iOS and iPadOS 

Article

# Inspecting iOS and iPadOS

Inspect webpages, Service Workers, Home Screen web apps, extensions, and content inside apps on iOS and iPadOS devices and simulators from a connected Mac.

## Overview

Web content on iOS and iPadOS is inspectable when you connect the device to your Mac. You can also use simulators on macOS to test your webpages and apps without a physical device. To learn more about device simulators, see Installing Xcode and Simulators.

## Enabling inspecting your device from a connected Mac

Before you can connect your device to a Mac to inspect it, you must allow the device to be inspected.

1.  Open the **Settings** app.

2.  Go to **Apps** \> **Safari**.

3.  Scroll down to **Advanced**.

4.  Enable the **Web Inspector** toggle.

Now, connect the device to your Mac using a cable. In Safari, the device will appear in the Develop menu.

Important

You may need to trust the Mac you connect your device to when the device prompts you before it appears in the **Develop** menu on your Mac.

### Connecting over the network

In addition to being able to inspect devices over a wired connection, you can also connect to your device over Wi-Fi or another network connection. To enable connecting over the network, you must first have enabled **Web Inspector** on your device and connected it to your Mac using a cable. Then, you can enable **Connect via Network** from the device’s submenu in the **Develop** menu. Alternatively, you can also connect to the device using Xcode.

### iOS and iPadOS simulators

**Web Inspector** is always enabled for simulators, and currently booted simulators will appear in the **Develop** menu just like connected devices.

## Inspecting a webpage

Webpages you open in Safari in iOS and iPadOS appear in a submenu for the connected device of the **Develop** menu of Safari on a connected Mac. Safari groups webpages and other content by app, making it easier to find the webpage you want to inspect.

Find the webpage you want to inspect, then select it to open a new Web Inspector window. This window continues inspecting the tab you started inspecting, including across navigations. If you close the tab in iOS or iPadOS, the Web Inspector window disappears.

For webpages, some additional options are available only while inspecting a connected device or a simulator to allow you to override the user agent, disable cross-origin restrictions, disable site-specific quirks, and more. See Device Settings.

## Inspecting a service worker

Service Workers are shared between webpages and don’t necessarily belong to any individual webpage. For this reason, they are inspectable separately from webpages in Safari.

You can only inspect service workers that are currently running. To inspect service workers, open the **Develop** menu, find the menu item for the visionOS device you want to inspect, and select them from the **Service Workers** section near the bottom of the menu. This section doesn’t appear if there aren’t any service workers currently running.

## Inspecting Home Screen web apps

When a Home Screen web app is in the foreground, you can inspect it from the **Develop** menu. Find the menu item for the iOS or iPadOS device you wish to inspect, and then find the web app’s URL in the **Home Screen Web Apps** section near the bottom of the menu.

## Inspecting extensions

Extensions can run scripts or create webpages in several places, and how you inspect them varies depending on the content. Learn more about debugging web extensions…

### Content scripts

To debug the scripts that web extensions inject into webpages, first inspect the webpage. Open Web Inspector, then click the Sources tab and select your content script file from the Extension Scripts folder at the lower left. Select your extension’s execution context using the selector in the lower-right corner of the inspector. Set breakpoints by clicking the gutter with line numbers in the source view. Inspect other source files for your extension, such as style sheets, in the Sources area at the lower left.

### Background scripts

To debug background scripts, open the **Develop** menu, find the menu item for the iOS or iPadOS device you wish to inspect, and then find the item with the name of the extension, “**Extension Background Page**”, and the file name of the background script.

### Toolbar pop-up

To debug your extension’s pop-up, open your pop-up on the device. Now from the **Develop** menu find the menu item for the iOS or iPadOS device you wish to inspect, and then find the item with the name of the extension, “**Extension Pop-up Page**”, and the file name of the pop-up’s HTML.

## Inspecting JavaScript and webpages in apps

You can make WKWebViews and JSContexts in apps inspectable, allowing anyone who enables **Web Inspector** on the device to inspect them. Content you can inspect appears in a submenu for the connected device of the **Develop** menu of Safari on a connected Mac. Safari separates webpages and JavaScript contexts by app, making finding the content you want to inspect easier.

Learn more about Enabling inspecting content in your apps.

## See Also

### Inspecting content

Inspecting Safari on macOS

Inspect webpages, Service Workers, and extensions in Safari on macOS.

Inspecting visionOS

Inspect webpages, service workers, extensions, and content inside apps in visionOS from a Mac on the same network.

Inspecting tvOS

Inspect JavaScript and TVML content on tvOS from a Mac on the same network.

Enabling inspecting content in your apps

Enable the inspection of webpages and JavaScript in apps you develop when inspected from a connected Mac.

