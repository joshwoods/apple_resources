

- Xcode
- Debugging
- Metal debugger
-  Debugging the shaders within a draw command or compute dispatch 

Article

# Debugging the shaders within a draw command or compute dispatch

Identify and fix problematic shaders in your app using the shader debugger.

## Overview

If you notice any visual artifacts while running your app, such as missing geometry or invalid pixels, you can use the shader debugger to investigate problematic shaders. Step through your shader source code and inspect variable values until you discover the problem. Then, just edit the shader source and reload the shader to verify your fix.

Important

Include source code when you capture a Metal workload because the shader debugger needs it to function correctly. For more information, see Building your project with embedded shader sources.

### Debug your shader

To begin debugging a shader, select the draw command or compute dispatch of interest in the Debug navigator. Then, click the Shader Debugger button in the debug bar to begin debugging any of the associated shaders for the currently bound pipeline state.

The shader debugger opens a dialog that includes a tab for each shader type in use so you can easily select the shader region of interest. For example, if your draw command has a vertex and fragment shader, the dialog includes Vertex and Fragment tabs.

The Vertex tab shows the geometry of your draw command. You can immediately start debugging your vertex shader by clicking the Debug button on the bottom right because the shader debugger automatically selects the first vertex.

For more information, see Inspecting the geometry of a draw command.

The dialog includes tabs for Mesh and Object, if applicable, instead of the Vertex tab when a draw command uses a mesh-based pipeline state.

The Mesh and Object tabs show the geometry of your draw command. You can immediately start debugging your mesh or object shaders by clicking the Debug button on the bottom right because the shader debugger automatically selects the first mesh grid and its first mesh.

You can set the threadgroup position that produced a mesh in the thread selector by clicking the Mesh tab and selecting a mesh in the table or the geometry view. You can also set the thread position that produced a vertex in a mesh by choosing Thread Position for Vertex and selecting a vertex in the table or the geometry view. Alternatively, you can set the thread position that produced a primitive or an index in a mesh by choosing Thread Position for Primitive or Index.

You can set the threadgroup position that produced a mesh grid in the thread selector by clicking the Object tab and selecting a mesh grid in the table or the geometry view.

For more information, see Inspecting the geometry of a draw command.

The Fragment tab shows the first attachment of your draw command, and hides other attachments by default. You can immediately start debugging your fragment shader by clicking the Debug button on the bottom right because the shader debugger automatically selects a pixel within a debuggable region. Alternatively, you can select a different pixel, change the visible attachments, and so on.

For more information, see Inspecting the attachments of a draw command.

If you select a compute dispatch rather than a draw command, you can immediately start debugging your compute shader by clicking the Debug button on the bottom right because the shader debugger automatically selects the first threadgroup.

You can also expand the Functions to Debug option to select a subset of functions within your shader source. Using a subset of functions can dramatically decrease the amount of the shader debugger’s initial processing.

You can also select a subset of functions in the Vertex, Mesh, Object, and Fragment tabs by clicking Debug while holding down the Option key.

### Step through your shader code

After you click the Debug button, the shader debugger displays the shader source in the Shader editor (see Inspecting shaders).  
The call tree on the left shows each executed line in your shader. The values of the variables appear to the right of each shader line of source code in the Shader editor. For example, in the screenshot below, you can see that the `in` variable has a value containing `721.5`, `815.5`, and so on.

If your shader is producing incorrect results, you can examine the value of variables on each line until you see an unexpected value that indicates the cause of the problem. Use the call tree to quickly inspect your shader:

When you select a line in the call tree, its corresponding line of source code in the Shader editor to the right appears with a green highlight. This line is also referred to as the *location of the playhead*. Use your keyboard arrow keys in the call tree to advance the playhead through your code one line at a time. As you step through the call tree, the playhead follows along in the source code in the Shader editor.

| Arrow key   | Stepping direction |
|-------------|--------------------|
| Down Arrow  | Steps forward      |
| Up Arrow    | Steps backward     |
| Right Arrow | Steps in           |
| Left Arrow  | Steps out          |

Alternatively, you can change the playhead location by clicking any line in the Shader editor, and the shader debugger moves to the corresponding function in the call tree.

### Iterate through loops

Unlike a traditional CPU debugger, the shader debugger shows the value of all variables at the same time, with no need to step to the next line. If you decide not to use the call tree to iterate through loops, you can switch the visible loop iteration directly within the Shader editor. Click the Loop Iteration tab on the right above the loop, just before the variables sidebar. When you select a different iteration, the variables within the sidebar update to reflect their values during that iteration.

### Inspect variable values

To inspect the value of a variable, move the pointer over it. For example, in the screenshot below, hovering over `linearSampler` shows the sampler properties in a popover.

Alternatively, you can toggle the Preview button in the variables sidebar to show the value inline with the source. This is useful if you want to compare the values of multiple variables simultaneously.

If a variable has nested properties, you can disclose them in a cascading fashion.

This enables you to dive in to an object’s data by showing you more than the Shader editor can fit in the right sidebar.

In addition to the selected pixel or thread, the shader debugger also shows the variable values for nearby pixels, or other threads within the threadgroup, in what is known as the *region of interest*. When you expand a variable preview, the shader debugger shows the values of variables for all pixels or threads within the region of interest.

Tip

The region of interest appears in the Attachments viewer as a fluorescent orange square (see Inspecting the attachments of a draw command), and in the Geometry viewer as an orange vertex (see Inspecting the geometry of a draw command).

Use this rendering to visually check that the variable is the value you expect. For graphical data, the visualization can be easier to verify than numerical data alone. Move the pointer over a pixel or thread to see the variable value for it. Then, you can click the pixel or thread to select it. The Shader editor automatically changes the variables in the variables sidebar to reflect their values during the execution of the shader when using the newly selected pixel or thread.

In the preview, the mask shows the pixels or threads within the region of interest that executed the line of code. Consider the example below, where the fragment shader branches depending on the vertex in-position. In the mask, the pixels within the region of interest that passed the condition appear with a white color, and pixels that didn’t pass the condition appear with a black color.

### Update your shader

After changing a shader, you can update the captured frame with the new source code by clicking the Reload Shaders button in the debug bar.

After updating the captured frame, the shader debugger does the following:

- Updates variable views to show their new values.

- Redraws attachments in the assistant editor.

- Maintains your place in the captured frame, which provides an interactive environment to enhance your shader development and debugging.

Important

Changes to your shader source only exist within the shader debugger. Your original source code doesn’t change. If your shader results look correct after reloading the shader, make sure that you copy your changes to your original shader source code.

If your shader is producing correct results, but taking a long time to run, consider profiling your Metal workload and inspecting the shader source in the Shader editor. For more information, see Inspecting shaders.

## See Also

### Metal command analysis

Inspecting the bound resources for a command

Discover issues by examining the bound resources at any point in an encoder.

Inspecting the geometry of a draw command

Find problems in your app’s vertex, object, or mesh function by examining the current geometry.

Inspecting the attachments of a draw command

Discover attachment issues by inspecting individual pixels and samples.

Analyzing draw command and compute dispatch performance with GPU counters

Identify issues within your frame capture by examining performance counters.

Analyzing draw command and compute dispatch performance with pipeline statistics

Identify issues within your frame capture by examining pipeline statistics.

