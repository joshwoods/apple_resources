

- Dispatch
-  Dispatch Data 

API Collection

# Dispatch Data

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

## Overview

The memory buffer managed by this object may be a single contiguous block of memory, or it may consist of multiple discontiguous blocks. For the discontiguous case, the dispatch data object makes it appear as if the memory is contiguous.

## Topics

### Creating a Dispatch Data Object

typealias dispatch_data_t

An immutable object representing a contiguous or sparse region of memory.

## See Also

### System Event Monitoring

class DispatchSource

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

Dispatch Source

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

class DispatchIO

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

struct DispatchData

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

struct DispatchDataIterator

A byte-by-byte iterator over the contents of a dispatch data object.

Dispatch I/O

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

protocol DispatchSourceProtocol

Defines a common set of properties and methods that are shared with all dispatch source types.

