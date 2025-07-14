

- SpriteKit
- Nodes for Scene Building
- SKVideoNode
-  Adding a Video to a Scene 

Article

# Adding a Video to a Scene

Play video in your scene by adding a video node.

## Overview

A video node renders a video at a given size and location in your scene with no exposed player controls. You might use a video node to animate visual behaviors that would be expensive to define using a collection of textures.

Be aware that a video node offers only a subset of the features available to the SKSpriteNode class. The following are a video node’s relevant limitations:

- A video node is always scaled proportionally.

- A video node cannot be colorized. However, it can be added as a child of a SKEffectNode to add Core Image filters for color treatments and other effects.

- A video node always uses an alpha blend mode.

- A video node cannot use custom shaders or lighting.

When a video node is created, its size property is initialized to the base size of the video content, but you can change it. The video content is automatically stretched to the new size. As with a sprite node, the anchorPoint property defines where the content is displayed relative to the node position.

The following code initializes the video node using a video file stored in the app bundle and then adds the node to the scene. It calls the node’s play() method to start the video playback.

- Swift
- Obj-C

```
let sample = SKVideoNode(fileNamed: "sample.mov")
sample.position = CGPoint(x: frame.midX,
                          y: frame.midY)
addChild(sample)
sample.play()
```

```
SKVideoNode *sample = [SKVideoNode videoNodeWithFileNamed:@"sample.mov"];
sample.position = CGPointMake(CGRectGetMidX(self.frame),
                              CGRectGetMidY(self.frame));
[self addChild: sample];
[sample play];
```

You control playback using the node’s play() and pause() methods.

If you need more precise control over the video playback behavior, you can use AVFoundation to create an AVPlayer object for your video content and then use this object to initialize the SKVideoNode node. Then, instead of using the node’s playback methods, you use the AVPlayer object to control playback. The video content is automatically displayed in the video node. For more information, see AVFoundation Programming Guide.

