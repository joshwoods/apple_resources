

- SpriteKit
- SKScene
-  Using Audio Nodes with the Scene’s Listener 

Article

# Using Audio Nodes with the Scene’s Listener

Add audio to your scene, and optionally give it 2D-positional mixing characteristics.

## Overview

The simplest way to add audio to a SpriteKit scene is to add a child SKAudioNode to it:

```
let audio = SKAudioNode(fileNamed: "drums.mp3")

spriteKitViewController.scene.addChild(audio)

```

However, if you define the presented scene’s listener, its audio nodes are played back with positional sound mixing. For example, if you set the scene’s `listener` to be the scene’s `camera` and then add audio nodes as children to various parent nodes in the scene, the further away the parent nodes are from the center of the screen, the quieter their audio will be played.

## See Also

### Adding Positional Audio

var listener: SKNode?

A node used to determine the position of the listener for positional audio in the scene.

var audioEngine: AVAudioEngine

The AVFoundation audio engine used to play audio from audio nodes contained in the scene.

