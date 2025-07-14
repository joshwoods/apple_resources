

- Xcode
- Debugging
- Metal debugger
-  Analyzing Apple GPU performance using counter statistics 

Article

# Analyzing Apple GPU performance using counter statistics

Optimize performance by examining counters for individual passes and commands.

## Overview

Important

The Performance counters feature is only applicable to Apple GPUs. For other GPU architectures, see Analyzing non-Apple GPU performance using counter statistics.

The Performance counters show performance statistics from your app’s passes or commands in the GPU trace. These counters measure hardware-related activities on the GPU, ranging from memory bandwidth to the number of vertices, the number of rasterized fragments, and the texture-filtering limiter and utilization percentages.

The Metal debugger collects data from the passes running without overlap, so only one pass runs at a time on the device when the profiler measures the performance. Additionally, it includes deterministic counters that don’t vary by time, such as the number of vertices in a render pass.

### View different counter sets for passes or commands

At the top of the graph, you can click the Encoders or the GPU Commands tab to choose to view the counters by pass or command granularity. Then, you can choose which counter set to use for viewing the collection of counters. In addition, clicking the Edit Counters button on the right allows you to create counter sets or to customize existing ones to suit your performance optimization workflow.

### View performance counters in the assistant editor

The assistant editor allows you to see additional information for individual passes and commands. You can enable the assistant editor by clicking the Adjust Editor Options button and choosing the Assistant option.

Selecting a pass or command shows its performance counters in the assistant editor. If you see something other than performance counters, you can select Performance from the drop-down menu at the top left of the editor.

The performance counters in the assistant editor let you inspect all the counters for a specific pass or command. By analyzing values that may be hotspots, counters can suggest a specific cause of your app’s performance problem. For example, if the number of vertices is twice as high as you expect, it’s likely that your code has duplicate meshes or render encoder draw calls.

For more information, see Analyzing draw command and compute dispatch performance with GPU counters.

### View pipeline statistics for a command

Selecting a command allows you to look at its pipeline statistics in the assistant editor. You can select Pipeline Statistics from the Assistant Editor drop-down menu to view information about the pipeline state and its performance statistics.

The pipeline statistics in the assistant editor let you look at compiler metrics and execution timing. The top portion of the assistant editor area lists the time each pipeline stage took to complete in separate categories. Below, it lists the commands that use the same pipeline stage, as well as their shader GPU time.

For more information, see Analyzing draw command and compute dispatch performance with pipeline statistics.

### Optimize your workload

There are a few interesting metrics you can investigate when beginning to optimize your workload:

Counters in the Performance Limiters counter set  
Use limiters as clues to offload work to underutilized subsystems on the GPU to help eliminate stalls in a particular subsystem. For more information, see Reducing shader bottlenecks.

Vertices counter in the Vertices counter set  
Check whether the number of vertices from a render pass or a draw command matches what you expect.

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

Analyzing Apple GPU performance with performance heat maps

Gain insights to SIMD group performance by inspecting source code execution.

Analyzing Apple GPU performance using the shader cost graph

Discover potential shader performance issues by examining pipeline states.

Analyzing non-Apple GPU performance using counter statistics

Optimize performance by examining counters for individual passes and commands.

