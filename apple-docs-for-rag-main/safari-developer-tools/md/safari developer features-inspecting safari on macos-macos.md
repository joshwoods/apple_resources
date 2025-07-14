

- Safari Developer Features
-  Inspecting Safari on macOS 

Article

# Inspecting Safari on macOS

Inspect webpages, Service Workers, and extensions in Safari on macOS.

## Overview

Safari supports inspecting all webpages, Service Workers, and extensions. The way in which you inspect content depends on the type of content.

## Inspecting a webpage

In Safari, there are two ways to begin inspecting a webpage.

The first is via the Develop menu. With the webpage you wish to inspect frontmost in Safari, go to the **Develop** menu and choose **Show Web Inspector** (⌥⌘I). Web Inspector will then appear, and will be inspecting the webpage.

The second was to show Web Inspector is to right click on the webpage and choose **Inspect Element** from the context menu. Web Inspector will then appear, and will have automatically highlighted the element you clicked on on the webpage.

Once opened, Web Inspector will continue to inspect the tab for which it was opened, even as you navigate to other pages in that tab.

## Inspecting a service worker

Service Workers are shared between webpages and don’t necessarily belong to any individual webpage. For this reason, they are inspectable separately from webpages in Safari.

When a service worker is running, you can inspect it by going to the **Develop** menu, selecting **Service Workers**, and then choosing the service worker you wish to inspect.

## Inspecting extensions

Extensions can run script or create webpages in several places, and how you inspect them varies depending on what the content is. Learn more about debugging web extensions…

### Content scripts

To debug the scripts that web extensions have injected into webpages, first inspect the webpage. Once Web Inspector is opened, click the Sources tab, and select your content script file from the Extension Scripts folder at the lower left. Then select your extension’s execution context by using the selector in the lower-right corner of the inspector. Set breakpoints by clicking the gutter with line numbers in the source view. Inspect other source files for your extension, such as style sheets, in the Sources area at the lower left.

### Background scripts

To debug background scripts, open the **Develop** menu and go to the **Web Extension Background Pages** submenu. From there, select background script for the extension you wish to inspect.

### Toolbar pop-up

To debug your extension’s pop-up, click the button for your extension in the Safari toolbar to display the pop-up. Control-click the pop-up and select **Inspect Element** to open Web Inspector for the pop-up.

## See Also

### Inspecting content

Inspecting iOS and iPadOS

Inspect webpages, Service Workers, Home Screen web apps, extensions, and content inside apps on iOS and iPadOS devices and simulators from a connected Mac.

Inspecting visionOS

Inspect webpages, service workers, extensions, and content inside apps in visionOS from a Mac on the same network.

Inspecting tvOS

Inspect JavaScript and TVML content on tvOS from a Mac on the same network.

Enabling inspecting content in your apps

Enable the inspection of webpages and JavaScript in apps you develop when inspected from a connected Mac.

