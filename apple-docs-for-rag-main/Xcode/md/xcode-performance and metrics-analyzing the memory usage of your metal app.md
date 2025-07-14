

- Xcode
- Performance and metrics
-  Analyzing the memory usage of your Metal app 

Article

# Analyzing the memory usage of your Metal app

Keep your app alive in the background by managing its memory footprint.

## Overview

Instruments provides the Game Memory template to help you understand the memory growth in your Metal app. Keeping a small memory footprint allows the system to keep the app alive in the background longer, especially on devices with more constrained memory capacity. For more information, see Profile and optimize your game’s memory.

### Open the Game Memory template

Start the memory analysis from your Xcode project by choosing Product \> Profile, or by pressing Command-I. Alternatively, you can launch Instruments and then select the process from the drop-down list.

In the Template Selection window, select Game Memory.

### Get to know the instruments

Allocations  
Analyzes the memory life cycle of a process’s allocated blocks, and can record reference-counting events.

Metal Resource Events  
Records Metal GPU resource allocations, such as textures and buffers.

VM Tracker  
Tracks the virtual memory space of a process over time, identifying regions by tag and reporting usage statistics.

Virtual Memory Trace  
Tracks virtual memory activity per thread.

Metal Application  
Records Metal app events.

GPU  
Records GPU events.

### Record an Instruments capture

Begin collecting the data by clicking the Record button.

Within your app, perform the actions that reproduce the memory problem, and then click the Record button to stop recording.

### Analyze your app’s memory allocations

The Game Memory template shows both memory allocations and memory footprint.

Memory allocations occupy space in the virtual memory address space. When your app allocates memory, these new allocations may not immediately take up space on physical memory. It’s not until your app uses these allocations that they consume physical memory.

The Allocations track provides a detailed view of memory allocations, their sizes, and object reference counts.

Note

The Allocations track doesn’t include Metal resources with private storage mode — only managed and shared storage modes.

The Statistics view in the bottom detail area displays the categories of memory allocations. At the top of the Category column, there are three umbrella categories that summarize all allocations:

All Heap & Anonymous VM  
Includes everything.

All Heap Allocations  
Includes dynamically allocated buffers that may contain resources.

All Anonymous VM  
Includes interesting VM regions that may be dirty. You can also find some Metal-related memory here.

Below them, you can find more detailed categories. Metal resource allocations are in the `VM: IOAccelerator` category, and drawables are in `VM: IOSurface`.

To inspect the individual allocations in a category, click the arrow button next to the category name in the table.

After selecting a category, you can sort the table by the Size column to find the largest memory allocation during the selected time range.

You can also select an allocation in the list to view its description and stack trace in the inspector on the right.

### Analyze Metal resource allocations

The Metal Resource Events track displays a history of all Metal-specific resource allocations and deallocations, along with their labels (see Naming resources and commands).

The Resource Events view in the bottom detail area lists the resource allocation and deallocation events. It includes events from created or destroyed resources in the selected time range. Not all resources in the list persisted until the end of the time range.

### Analyze your app’s total virtual memory footprint

The Allocations track and the Metal Resource Events track both highlight memory allocations. However, allocations don’t always translate to memory footprint. The VM Tracker track shows the noncompressed and compressed/swapped dirty memory that together make up your app’s memory footprint.

Memory operates on the granularity of pages, and those pages can be either clean or dirty.

Clean memory  
Includes memory-mapped files and read-only frameworks.

Dirty memory  
Includes heap-allocated memory and written symbols in frameworks.

To conserve the amount of physical memory that your app uses, the system may compress or swap out some dirty pages that your app hasn’t accessed recently.

Important

The system charges your app for any compressed/swapped memory based on its orginal size before compression.

The center timeline area graphs the following metrics:

Dirty Size  
The amount of noncompressed dirty memory.

Swapped Size  
The amount of compressed/swapped dirty memory in its original size before compression.

Resident Size  
The amount of resident memory.

The corresponding columns are also available in the Summary view of the bottom detail area. There, you can expand the VM region types. In the mapped file type in the screenshot below, you can see the memory-mapped file of the bistro scene that the Modern Renderer app loaded:

## See Also

### Graphics

Analyzing the performance of your Metal app

Ensure consistent, smooth rendering by profiling your app’s frame time.

