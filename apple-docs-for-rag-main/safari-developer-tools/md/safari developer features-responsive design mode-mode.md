

- Safari Developer Features
-  Responsive Design Mode 

Article

# Responsive Design Mode

Use Responsive Design Mode to test your `media` queries and other dynamic styles to ensure your webpages look great on any screen.

## Overview

Responsive Design Mode lets you quickly preview how your webpage responds to changes in width and height, as well as differences in the pixel ratio of displays. Use Responsive Design Mode to ensure all visitors to your webpage get a great experience, no matter the size of their screen.

## Opening Responsive Design Mode

While focused on the webpage you want to test in Responsive Design Mode, choose **Enter Responsive Design Mode** (⌃⌘R) from the Develop menu.

Tip

You can use Responsive Design Mode with Web Inspector to debug your page’s layout while resizing the page in Responsive Design Mode.

## Using Responsive Design Mode

### Viewport Size Presets

You can pick from a list of viewport size presets to quickly preview how your webpage layout will adapt to various device screen sizes.

Viewport size presets offer a good approximation, but they don’t represent exact layout, rendering, and behavior as experienced on an actual device. For example, the webpage layout on a device might be influenced by the browser address bar, the on-screen keyboard, or by device-specific behavior for form fields. For a more accurate preview, use the Open with Simulator menu to view your webpage in a Simulator.

### Rotate Viewport

Use this button to swap the dimensions for the current viewport. You can use this to check your webpage’s layout in both orientations of a viewport.

### Size

The current effective size of the viewport, in screen points. You can click on the width or height to begin editing the specific dimension. You can also grab the handles on the left, bottom, and right sides of the viewport to quickly resize to any dimension, or grab one of the bottom corners to resize in both dimensions simultaneously.

When you change the size of the viewport, the dimensions are saved to the viewport preset labeled as **Custom size**.

### Zoom

The current percentage of actual size of the viewport. Normally, this will be 100% which means each pixel of the web content is visible on screen. When you enlarge the viewport to be larger than the window you are currently using, the zoom decreases, indicating that some pixels of web content are now being lost. The zoom is not directly editable, it changes based on the viewport size and the window size.

### Pixel Ratio

The current pixel ratio at which to render content. Some devices and monitors may have different pixel densities, and different images can be loaded and different styles applied to pages. For example, a page may define multiple image resources at different pixel ratios in order to deliver the highest quality necessary without delivering a file that is larger than necessary

```
```

```
```

You may also want to provide alternative styles for displays with different pixel ratios, like thinner lines on a 2× display. You can use a CSS media query for these kinds of adaptive style changes:

```
```

### Open with Simulator

iOS, iPadOS, and visionOS have different rendering behaviors than macOS, as they are optimized for different form-factor devices and interaction models. It is important to test your webpages in such an environment, and simulators provide an accurate way to do so without additional devices. If you don’t have Xcode installed, or want to add more simulators, see Installing Xcode and Simulators and Adding additional simulators.

## See Also

### Tools

Develop menu

Access tools for debugging webpages in Safari, as well as tools for debugging web content in other apps and on other devices.

Web Inspector

Use Web Inspector to inspect and debug your HTML, CSS, and JavaScript.

WebDriver

Use WebDriver to write robust, comprehensive tests and run them against any browser that has a WebDriver-compliant driver, including Safari.

