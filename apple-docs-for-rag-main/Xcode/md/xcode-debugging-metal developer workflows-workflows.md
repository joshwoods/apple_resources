

- Xcode
- Debugging
-  Metal developer workflows 

# Metal developer workflows

Locate and fix issues related to your app’s use of the Metal API and GPU functions.

## Overview

Metal comes with a comprehensive suite of advanced developer tools to help you debug and optimize your Metal apps.

### Runtime diagnostics

You can enable API Validation when running your app to check for incorrect Metal API usage. For more information, see Validating your app’s Metal API usage.

Enable Shader Validation when running your app to check for issues like out-of-bounds memory access, missing `useResource` calls, and stack overflows. For more information, see Validating your app’s Metal shader usage.

The Metal Performance HUD offers a visual overlay to catch performance issues while your app is running. For more information, see Monitoring your Metal app’s graphics performance.

### Runtime performance analysis

The Metal system trace tool in Instruments provides a visual timeline of the parallel work on the CPU and the GPU, and the memory usage of your Metal app.

You can begin profiling with the Game Performance template (see Analyzing the performance of your Metal app) or the Game Memory template (see Analyzing the memory usage of your Metal app).

### Advanced Metal debugging and profiling

The Metal debugger in Xcode provides advanced tools for debugging and profiling your Metal app.

You can get summaries of your Metal workload with the Dependencies viewer and the Memory viewer, inspect individual resources, and selectively debug your shaders. For more information on debugging, see Investigating visual artifacts.

In addition, you can optimize your Metal app by drilling down performance bottlenecks with the Performance timeline and the per-line shader profiling results. For more information on profiling, see Optimizing GPU performance.

Learn more about Metal debugger.

## Topics

### Project preparation for debugging

Make your Metal app easier to debug by taking a few extra steps as you develop your code.

Building your project with embedded shader sources

Prepare to debug your project’s shaders by including source code in the build.

Naming resources and commands

Enhance the debugging of your Metal app using labels and grouping.

Creating and using custom capture scopes

Capture specific GPU commands by using custom capture scopes.

### Runtime diagnostics

Learn how to use runtime tools to discover potential issues in your Metal app.

Inspecting live resources at runtime

Validate your resources by viewing the contents of your textures and buffers while debugging your Metal app.

Validating your app’s Metal API usage

Catch runtime issues in your Metal app using API Validation.

Validating your app’s Metal shader usage

Catch common shader runtime issues using Shader Validation while your app is running.

Monitoring your Metal app’s graphics performance

Catch performance issues using the Metal Performance HUD while your app is running.

### Counters

Get references for the set of performance metrics available across Metal tools.

Finding your Metal app’s GPU occupancy

Understand the GPU usage for executing shaders by using occupancy.

Reducing shader bottlenecks

Identify and minimize congestion points in a GPU’s subsystems by checking its limiter and utilization counters.

Measuring the GPU’s use of memory bandwidth

Check whether your Metal app correctly reads and writes to memory by measuring the GPU’s memory bandwidth.

## See Also

### Graphics

Metal debugger

Debug and profile your Metal workload with a GPU trace.

