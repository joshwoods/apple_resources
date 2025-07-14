

- Xcode
- Debugging
- Metal developer workflows
-  Monitoring your Metal app’s graphics performance 

Article

# Monitoring your Metal app’s graphics performance

Catch performance issues using the Metal Performance HUD while your app is running.

## Overview

The Metal Performance HUD (heads-up display) adds a real-time overlay to your app that displays and, optionally, logs common graphics performance information. The overlay helps you spot subtle performance issues, such as large variations in rendering time, so you can find the perfect scope to capture in Xcode (see Capturing a Metal workload in Xcode) or in Instruments (see Analyzing the performance of your Metal app).

The GPU and resolution appear at the top of the HUD, along with the display scaling factor, refresh rate, and an indicator for whether the present mode is `direct` or `composited`.

The middle section of the HUD shows three rows of information, each with three columns:

- The first column contains the mean values from the last 1.5 seconds of the frames per second (FPS), the present-to-present interval (Pre), and the GPU time (GPU).

- The second column contains the minimum values from the last 1.5 seconds of FPS, Pre, and GPU.

- The third column contains the maximum values from the last 1.5 seconds of FPS, Pre, and GPU.

When minimum and maximum values vary by more than 15% from the average, they appear with a red highligt for easier identification.

The bottom section of the HUD shows the app’s overall memory footprint, the GPU memory footprint, and a graph of the last 200 frames of the present-to-present interval (Pre) and the GPU time (GPU).

For more information, see Discover Metal Performance HUD.

### Enable the Metal Performance HUD in Xcode

Follow these steps to enable the Metal Performance HUD using the runtime diagnostics options in the scheme settings:

1.  In the Xcode toolbar, choose Edit Scheme from the Scheme menu. Alternatively, choose Product \> Scheme \> Edit Scheme. 

2.  In the scheme action panel, select Run.

3.  In the action setting tab, click Diagnostics.

4.  Select Show Graphics Overview to enable the Metal Performance HUD, and click Close. 

Now, the Metal Performance HUD runtime is enabled each time you run your scheme.

### Enable logging in Xcode

You can also optionally enable the output of per-frame statistics to the console by selecting the Log Graphics Overview option.

Note

You need to select both the Show Graphics Overview and the Log Graphics Overview options to output per-frame statistics.

Then, as your app is running, once per second (or more frequently at high present rates due to vsync-off or high-refresh and VRR displays), the HUD writes data in the following format to the console:

```
metal-HUD: ,,,,,...,
```

For example, the HUD wrote the following data to the console while running the Rendering a Scene with Deferred Lighting in Swift sample code project:

### Enable the HUD and logging with environment variables

You can enable the Metal Performance HUD and logging by setting the following environment variables on your Metal app:

MTL_HUD_ENABLED=1  
Enables the Metal Performance HUD.

MTL_HUD_LOG_ENABLED=1  
Enables logging of per-frame statistics. Requires `MTL_HUD_ENABLED=1`.

Alternatively, you can enable the HUD and logging programmatically as follows:

1.  Add `MetalHudEnabled` to your app’s `Info.plist` file.

2.  Either set `MetalHUDForceEnabled=1` in your app’s UserDefaults, or configure your `CAMetalLayer` instance’s `developerHUDProperties` dictionary with the following:

    ```
    myMetalLayer.developerHUDProperties = [
        "mode": "default",
        "logging": "default"
    ]
    ```

### Enable the HUD and logging on a device

You can enable the Metal Performance HUD and logging on an iOS, iPadOS, or tvOS device in the Developer settings by following these steps:

1.  Open the Settings app.

2.  Select Developer.

3.  Under Graphics HUD, toggle the Show Graphics HUD option to enable the Metal Performance HUD.

4.  Toggle the Log Graphics Performance option to enable logging.

The Metal Performance HUD appears for apps you build and install yourself to your development devices.

Note

Your device needs to have a development provisioning profile for the Developer options to appear in the Settings app.

The following screenshot shows the options in iOS:

The following screenshot shows the options in tvOS:

## See Also

### Runtime diagnostics

Inspecting live resources at runtime

Validate your resources by viewing the contents of your textures and buffers while debugging your Metal app.

Validating your app’s Metal API usage

Catch runtime issues in your Metal app using API Validation.

Validating your app’s Metal shader usage

Catch common shader runtime issues using Shader Validation while your app is running.

