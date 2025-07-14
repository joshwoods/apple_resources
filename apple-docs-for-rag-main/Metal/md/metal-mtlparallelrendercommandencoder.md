

- Metal
-  MTLParallelRenderCommandEncoder 

Protocol

# MTLParallelRenderCommandEncoder

An object that splits up a single render pass so that it can be simultaneously encoded from multiple threads.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLParallelRenderCommandEncoder : MTLCommandEncoder
```

## Overview

Your app does not define classes that implement this protocol. To create a MTLParallelRenderCommandEncoder object, call the makeParallelRenderCommandEncoder(descriptor:) method of the MTLCommandBuffer object that you want to encode the rendering commands into. Then, call the renderCommandEncoder method on this MTLParallelRenderCommandEncoder object to create one or more MTLRenderCommandEncoder objects. The subordinate MTLRenderCommandEncoder objects created encode their commands to the same command buffer and target the same MTLRenderPassAttachmentDescriptor object. The MTLParallelRenderCommandEncoder object ensures the attachment load and store actions only occur at the start and end of the entire rendering pass.

You can assign each MTLRenderCommandEncoder to its own thread and each can encode commands in parallel. You are responsible for any thread synchronization that is required. After all the subordinate encoders have finished encoding their commands, call endEncoding() to execute the commands. The rendering commands are executed in the order that the subordinate encoders were created.

## Topics

### Creating a Render Command Encoder

func makeRenderCommandEncoder() -> (any MTLRenderCommandEncoder)?

Create an object that encodes commands that perform graphics rendering operations and may be assigned to a different thread.

**Required**

### Setting Render Pass State

func setColorStoreAction(MTLStoreAction, index: Int)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given color attachment.

**Required**

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Specifies known store action options for a given color attachment.

**Required**

func setDepthStoreAction(MTLStoreAction)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given depth attachment.

**Required**

func setDepthStoreActionOptions(MTLStoreActionOptions)

Specifies known store action options for a given depth attachment.

**Required**

func setStencilStoreAction(MTLStoreAction)

Specifies a known store action to replace the initial MTLStoreAction.unknown value specified for a given stencil attachment.

**Required**

func setStencilStoreActionOptions(MTLStoreActionOptions)

Specifies known store action options for a given stencil attachment.

**Required**

## Relationships

### Inherits From

- MTLCommandEncoder
- NSObjectProtocol

## See Also

### Encoding a Render Pass in Parallel

enum MTLLoadAction

Types of actions performed for an attachment at the start of a rendering pass.

enum MTLStoreAction

Types of actions performed for an attachment at the end of a rendering pass.

struct MTLStoreActionOptions

Options that modify a store action.

