

- Xcode
- Debugging
- Metal debugger
-  Investigating visual artifacts 

Article

# Investigating visual artifacts

Discover, diagnose, and fix visual artifacts in your app with the Metal debugger.

## Overview

If you notice any visual artifacts while running your app, you can use the Metal debugger to find and investigate problematic pixels. First, configure your build to include shader source code (see Building your project with embedded shader sources). Then, take a frame capture of your app when you notice the visual artifact that you want to debug (see Capturing a Metal workload in Xcode).

After you have a frame capture, use the Debug navigator to find the draw command that contains the visual artifact, and use the Attachments viewer to find the pixel with the issue. Debug the pixel to launch the shader debugger, then step through your shader source code and inspect variable values until you discover the problem. Then, edit the shader source and reload the shader to verify your fix.

### Skim through render attachments in the Debug navigator

In the Metal debugger, navigate to a draw command that has the issue. As you move your pointer over rows in the Debug navigator on the left, the Metal debugger shows a preview of the first attachment. You can use this to quickly find any draw commands that warrant further inspection.

You also can filter the navigator to show only markers and commands so it’s easier to compare draw commands.

When you find the problematic draw command, click it to select it. The Metal debugger automatically shows your attachments in the assistant editor on the right.

### Inspect attachments for a draw command

Use the Attachments viewer to find any problematic pixels. You can scroll to zoom in, and drag to pan. For more information on the Attachments viewer, see Inspecting the attachments of a draw command.

Click the problematic pixel to select it, and then click the Debug button.

If the problematic pixel isn’t inside a debuggable region, it has a nongreen selection indicator (as with the blue indicator in the screenshot below). This means that the draw command didn’t write to that pixel and, therefore, you can’t debug it. Because the Attachments viewer remembers your zoom and position, you can quickly step through different draw commands in the Debug navigator to find the right one.

### Debug your fragment shader

The shader debugger displays the shader source in the Shader editor (see Inspecting shaders). The call tree on the left shows each executed line in your shader. The values of the variables appear to the right of each shader line in the shader source code. For example, in the screenshot below, you can see that the `in` variable has a value containing `721.5`, `815.5`, and so forth.

Step through your shader source code and inspect variable values until you discover the problem. Make changes to the shader source code, and then click the Reload Shaders button in the debug bar to refresh the variable values, along with the attachments.

If you still see visual artifacts, continue editing the shader and reloading it as needed until you solve the problem.

Important

Changes to your shader source code exist only within the Metal debugger. Your original shader source code doesn’t change.  
If your shader results look correct after reloading the shader, make sure that you copy your changes to your original shader source code.

To learn more, see Debugging the shaders within a draw command or compute dispatch.

## See Also

### Essentials

Capturing a Metal workload in Xcode

Analyze your app’s performance by configuring your project to use the Metal debugger.

Capturing a Metal workload programmatically

Analyze your app’s performance by invoking Metal’s frame capture.

Replaying a GPU trace file

Debug and profile your app’s performance using a GPU trace file in the Metal debugger.

Optimizing GPU performance

Find and address performance bottlenecks using the Metal debugger.

