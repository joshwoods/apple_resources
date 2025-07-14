

- Metal
- Render Passes
-  Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass 

Article

# Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass

Inform Metal when your app uses programmable sample positions for its depth render targets or copies MSAA depth data.

## Overview

A render or compute pass usually stores its target’s depth data in a compressed format. Any subsequent pass has to use the correct sample positions to decompress the data before reading it. You can store depth data in a representation that uses arbitrary sample positions (see Positioning Samples Programmatically).

Important

You can sample depth positions programmatically only on devices that support programmable sample positions (see areProgrammableSamplePositionsSupported).

When your app uses custom sampling positions, inform Metal by setting the MTLRenderPassColorAttachmentDescriptor or MTLRenderPassDepthAttachmentDescriptor instance’s storeActionOptions property to customSamplePositions. This setting tells Metal that any subsequent pass that reads the attachment may not know the sample positions the current pass uses to generate the data. Examples of a pass that can use custom sample positions include the following:

- A fragment shader that uses unique, programmable sample positions

- A blit pass that copies MSAA depth data to another resource

In this scenario, Metal may decompress the depth render target and store the uncompressed data.

Tip

Improve the performance of a pass if its programmable sample positions are the same for the next pass by setting the descriptor’s storeAction property to MTLStoreAction.store and clearing the customSamplePositions option from the storeActionOptions property.

## See Also

### Advanced Multisampling

Positioning Samples Programmatically

Configure the position of samples when rendering to a multisampled render target.

