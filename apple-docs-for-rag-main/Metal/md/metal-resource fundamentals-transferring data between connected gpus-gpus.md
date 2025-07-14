

- Metal
- Resource Fundamentals
-  Transferring Data Between Connected GPUs 

Article

# Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

## Overview

Starting with macOS 10.15, some Mac systems directly connect GPUs to each other, allowing you to quickly transfer data between them. These connections are not only faster, but they also avoid using the memory bus between the CPU and GPUs, leaving it available for other tasks. If your app uses multiple GPUs, test to see if they’re connected, and when they are, use the transfer mechanism described here.

When GPUs are connected to each other, they’re said to be in the same *peer group*. You determine whether a GPU is in a peer group by reading the device object’s peerGroupID property. A nonzero value indicates that the GPU is in a peer group.

- Swift
- Objective-C

```
func isMemberOfAnyPeerGroup(_ device: MTLDevice ) -> Bool
{
    return device.peerGroupID != 0
}
```

```
bool isMemberOfAnyPeerGroup(id device)
{
    return (device.peerGroupID != 0);
}
```

GPUs in the same peer group share the same peer group ID. 

- Swift
- Objective-C

```
func areMembersOfSamePeerGroup(_ deviceA:MTLDevice,_ deviceB: MTLDevice) -> Bool
{
    return isMemberOfAnyPeerGroup(deviceA) &&
           deviceA.peerGroupID == deviceB.peerGroupID
}
```

```
bool areMembersOfSamePeerGroup(id deviceA, id deviceB)
{
    return (isMemberOfAnyPeerGroup(deviceA) &&
            deviceA.peerGroupID == deviceB.peerGroupID);
}
```

You can get the list of all devices associated with a peer group by filtering on this ID.

- Swift
- Objective-C

```
func devicesInPeerGroup(_ peerGroupID: UInt64) -> [MTLDevice]
{
    if peerGroupID == 0
    {
        return []
    }
    let allDevices = MTLCopyAllDevices()
    return allDevices.filter({$0.peerGroupID == peerGroupID})
}
```

```
NSArray>* devicesInPeerGroup(uint64_t peerGroupID)
{
    if (peerGroupID == 0)
    {
        return @[];
    }
    return [MTLCopyAllDevices() filteredArrayUsingPredicate: [NSPredicate predicateWithFormat:@"SELF.peerGroupID == %uul", peerGroupID]];
}
```

### Copy Resources to the GPU that Needs to Access Them

In Metal, resources are created by device objects, and are always associated with the device object that created them. Peer groups don’t change that association. If a resource is associated with a device object, and you want to access it on another device object, you need to copy the data to a resource associated with the second device object.

To copy data between members of a peer group, make a *remote view* on the second GPU that’s connected to the resource you want to copy. A remote view is a resource object that contains no storage of its own; it references the storage on the original GPU. You can only use remote views to copy data; using them in other Metal commands results in an error.

### Create a Remote View of a Resource

To create a remote view of a resource, the device object you make the resource view on must share the same peerGroupID as the device object that created the resource. In addition, the resource must use the MTLStorageMode.private storage mode or be backed by an IOSurface.

To create a buffer view, call the makeRemoteBufferView(_:) method:

- Swift
- Objective-C

```
let remoteBufferView = sourceBuffer.makeRemoteBufferView(otherDevice)
```

```
id remoteBufferView = [sourceBuffer newRemoteBufferViewForDevice:otherDevice];
```

Similarly, to create a texture view, call the makeRemoteTextureView(_:) method.

- Swift
- Objective-C

```
let remoteTextureView = sourceTexture.makeRemoteTextureView(otherDevice)
```

```
id remoteTextureView = [sourceTexture newRemoteTextureViewForDevice:otherDevice];
```

### Copy Data Between Connected GPUs

Create a MTLBlitCommandEncoder and encode a copy command. The source for this copy command is the remote view object:

- Swift
- Objective-C

```
if let blitEncoder = commandBuffer.makeBlitCommandEncoder()
{
    blitEncoder.copy(from: remoteBufferView, sourceOffset: 0,
                       to: destinationBuffer, destinationOffset: 0,
                     size: remoteBufferView.allocatedSize)

    blitEncoder.copy(from: remoteTextureView,
                       to: destinationTexture)

    blitEncoder.endEncoding()
}
```

```
id blitEncoder = [commandBuffer blitCommandEncoder];
[blitEncoder copyFromBuffer:remoteBufferView sourceOffset:0
                   toBuffer:destinationBuffer destinationOffset:0
                       size:remoteBufferView.allocatedSize];
[blitEncoder copyFromTexture:remoteTextureView
                   toTexture:destinationTexture];
[blitEncoder endEncoding];
```

As shown in the following illustration, there are three resource objects: the original resource that contains the data, a remote view that references the data, and a resource that receives the data.

### Synchronize Access to Resources

Blit commands used in peer-to-peer transfers follow all of the usual synchronization rules on the GPU they’re performed on. However, they don’t automatically synchronize with any commands running on the source GPU. If you encode commands that modify the source resource, ensure that those commands are complete before executing the blit command to transfer the data to the other GPU. This is the same as what you do when transferring resources between GPUs through system memory.

To synchronize commands between different device objects, use shared events. See Synchronizing Events Across Multiple Devices or Processes and Implementing a Multistage Image Filter Using Heaps and Events.

## See Also

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

Choosing a Resource Storage Mode for Intel and AMD GPUs

Select an appropriate storage mode for your textures and buffers on AMD and Intel GPUs.

Copying Data to a Private Resource

Use a blit command encoder to copy buffer or texture data to a private resource.

Synchronizing a Managed Resource in macOS

Manually synchronize memory for a Metal resource in apps.

Reducing the Memory Footprint of Metal Apps

Learn best practices for using memory efficiently in iOS and tvOS.

