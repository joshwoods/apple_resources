

- SceneKit
-  SCNFieldForceEvaluator 

Type Alias

# SCNFieldForceEvaluator

The signature for a block that SceneKit calls to determine the effect of a custom field on an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNFieldForceEvaluator = (SCNVector3, SCNVector3, Float, Float, TimeInterval) -> SCNVector3
```

## Discussion

You use this type of block to create a custom physics field with the customField(evaluationBlock:) method. SceneKit calls your block once for each object in the field’s area of effect, on each step of the physics simulation.

Note

By default, one simulation step occurs for each frame rendered. For example, if your view renders at 60 frames per second and three bodies are in the field’s area of effect, SceneKit runs your block 180 times per second. To avoid reduced rendering performance, take care not to perform extensive computation in this block.

The block takes the following parameters:

position  
The position of the object affected by the field, in the local coordinate space of the node containing the field.

velocity  
The velocity of the object affected by the field, relative to the local coordinate space of the node containing the field.

mass  
The mass of the object affected by the field. (See the mass property for physics bodies and the particleMass property for particle systems.)

charge  
The electrical charge of the object affected by the field. (See the charge property for physics bodies and the particleCharge property for particle systems.)

time  
The elapsed time, in seconds, since the last simulation step.

Your block uses these parameters to compute and return an SCNVector3 force vector, which SceneKit then applies to the object affected by the field.

## See Also

### Constants

enum SCNPhysicsFieldScope

Options for defining the region of space affected by a physics field, used by the scope property.

