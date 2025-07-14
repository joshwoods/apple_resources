

- RealityKit
- Reality Composer
- Creating 3D Content with Reality Composer
-  Taking Control of Scene Anchoring 

Article

# Taking Control of Scene Anchoring

Create a more interactive user experience by choosing exactly where to anchor Reality Composer scenes.

## Overview

You might sometimes want to take direct control over anchoring in a Reality Composer scene. If, for example, multiple surfaces or objects in your scene are appropriate as anchors, you could let the user choose where to anchor the scene. Alternatively, you could create an algorithm that determines which of the available anchors to use, such as selecting the anchor closest to the center of the screen or the anchor that’s closest to the user. To allow for direct control over anchoring in a scene, you load it without anchoring information and then anchor it manually.

### Load the scene without anchoring information

Use one of these options:

- For synchronous loading, use load(contentsOf:withName:) instead of loadAnchor(contentsOf:withName:).

- For asynchronous loading, use loadAsync(contentsOf:withName:) instead of loadAnchorAsync(contentsOf:withName:).

This example shows the synchronous loading option:

```
func loadUnanchoredScene (filename: String,
                          fileExtension: String,
                          sceneName: String) -> (Entity & HasAnchoring)? {
    guard let realitySceneURL = createRealityURL(filename: filename,
                                                 fileExtension: fileExtension,
                                                 sceneName: sceneName) else {
        return nil
    }
    let loadedScene = try? Entity.load(contentsOf: realitySceneURL)

    return loadedScene
}
```

### Anchor the scene manually

When you load scenes without anchoring information, you can’t add them directly to a scene’s anchors. Instead, manually create a new AnchorEntity at the desired location, add your loaded scene as a child of the AnchorEntity, and then add the scene to the ARView scene anchors. For example, if you want to place your scene where the user taps, you can use raycast(from:allowing:alignment:) to look for a suitable surface, and then place it on the tapped surface if one exists.

```
@discardableResult
func addUnanchoredEntityWhereTapped(_ entity: Entity, 
                                    _ touchPoint:CGPoint)  -> Bool {
    let results = arView.raycast(from: touchPoint, 
                                 allowing: .estimatedPlane, 
                                 alignment: .horizontal)
        if let result = results.first {
            let anchorEntity = AnchorEntity(world: result.worldTransform)
            anchorEntity.addChild(entity)
            arView.scene.addAnchor(anchorEntity)      
            return true
        }
    return false
}
```

## See Also

### Scene anchors

Selecting an anchor for a Reality Composer scene

Decide which anchor is right for your scenes.

