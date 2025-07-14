

- Xcode
- Debugging
- Metal debugger
-  Analyzing non-Apple GPU performance using counter statistics 

Article

# Analyzing non-Apple GPU performance using counter statistics

Optimize performance by examining counters for individual passes and commands.

## Overview

Important

The Counters viewer feature isn’t applicable to Apple GPUs. For Apple GPUs, see Analyzing Apple GPU performance using a visual timeline and Analyzing Apple GPU performance using counter statistics.

The Counters viewer shows performance counters from your app’s passes or commands in the GPU trace. These counters measure hardware-related activities on the GPU, ranging from memory bandwidth to the number of vertices, the number of rasterized fragments, and the texture-filtering limiter and utilization percentages.

The Metal debugger collects data from the passes running without overlap, so only one pass runs at a time on the device when the profiler measures the performance. Additionally, it includes deterministic counters that don’t vary by time, such as the number of vertices in a render pass.

### View different counter sets for passes or commands

At the top of the graph, you can click the Encoder or the Draw tab to choose to view the counters by pass or command granularity. Then, you can choose which counter set to use for viewing the collection of counters.

### Find a pass with high shader GPU time

The height of the orange bar for each pass represents its shader GPU time. The tallest bar corresponds to the pass that took the longest time to complete. Minimize the duration of the long-running passes to optimize your app’s performance.

There are three render passes in the screenshot above, with the tallest bar for shader GPU time at the GBuffer Generation pass. You can move the pointer over the bar to view the time and other information. In the screenshot above, the shader GPU time for the GBuffer Generation pass reads 657.69 microseconds (μs).

### View performance counters in the assistant editor

The assistant editor allows you to see additional information for individual passes and commands. You can enable the assistant editor by clicking the Adjust Editor Options button and choosing the Assistant option.

Selecting a pass or command shows its performance counters in the assistant editor. If you see something other than performance counters, you can select Performance from the drop-down menu at the top left of the editor.

The performance counters in the assistant editor let you inspect all the counters for a specific pass or command. By analyzing values that may be hotspots, counters can suggest a specific cause of your app’s performance problem. For example, if the number of vertices is twice as high as you expect, it’s likely that your code has duplicate meshes or render encoder draw calls.

For more information, see Analyzing draw command and compute dispatch performance with GPU counters.

### View pipeline statistics for a command

Selecting a command allows you to look at its pipeline statistics in the assistant editor. You can select Pipeline Statistics from the Assistant Editor drop-down menu to view information about the pipeline state and its performance statistics.

The pipeline statistics in the assistant editor let you look at compiler statistics and runtime profiling statistics. The top portion of the assistant editor area lists the time each pipeline stage took to complete in separate categories. Below, it lists the commands that use the same pipeline stage, as well as their shader GPU time.

For more information, see Analyzing draw command and compute dispatch performance with pipeline statistics.

Sometimes, counters data may only hint at a problem, and you can benefit by leveraging additional Metal tools. For example, if your fragment shader time is unexpectedly high, you can use the Shader editor to discover which specific lines in your fragment shader are slowing down the execution. For more information, see Inspecting shaders.

## See Also

### Metal workload analysis

Analyzing your Metal workload

Investigate your app’s workload, dependencies, performance, and memory impact using the Metal debugger.

Analyzing resource dependencies

Avoid unnecessary work in your Metal app by understanding the relationships between resources.

Analyzing memory usage

Manage your Metal app’s memory usage by inspecting its resources.

Analyzing Apple GPU performance using a visual timeline

Locate performance issues using the Performance timeline.

Analyzing Apple GPU performance using counter statistics

Optimize performance by examining counters for individual passes and commands.

Analyzing Apple GPU performance with performance heat maps

Gain insights to SIMD group performance by inspecting source code execution.

Analyzing Apple GPU performance using the shader cost graph

Discover potential shader performance issues by examining pipeline states.

