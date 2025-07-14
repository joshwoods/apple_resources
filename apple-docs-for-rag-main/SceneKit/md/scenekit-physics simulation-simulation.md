

- SceneKit
-  Physics Simulation 

API Collection

# Physics Simulation

Add dynamic behaviors to scene elements; detect contacts and collisions; simulate realistic effects like gravity, springs, and vehicles.

## Topics

### Physics Bodies

class SCNPhysicsBody

The physics simulation attributes attached to a scene graph node.

class SCNPhysicsShape

An abstraction of a physics body’s solid volume for tuning collision detection.

### Collision and Contact Detection

protocol SCNPhysicsContactDelegate

Methods you can implement to respond when a contact or collision occurs between two physics bodies in a scene.

class SCNPhysicsContact

Detailed information about a contact between two physics bodies in a scene’s physics simulation.

### Physics in a Scene

class SCNPhysicsWorld

The global simulation of collisions, gravity, joints, and other physics effects in a scene.

class SCNPhysicsField

An object that applies forces, such as gravitation, electromagnetism, and turbulence, to physics bodies within a certain area of effect.

class SCNPhysicsBehavior

The abstract superclass for joints, vehicle simulations, and other high-level behaviors that incorporate multiple physics bodies.

### Joints

class SCNPhysicsHingeJoint

A physics behavior that connects two bodies and allows them to pivot around each other on a single axis.

class SCNPhysicsSliderJoint

A physics behavior that connects two bodies and allows them to slide against each other and rotate around their connecting points.

class SCNPhysicsBallSocketJoint

A physics behavior that connects two physics bodies and allows them to pivot around each other in any direction.

class SCNPhysicsConeTwistJoint

### Vehicle Simulation

class SCNPhysicsVehicle

A physics behavior that modifies a physics body to behave like a car, motorcycle, or other wheeled vehicle.

class SCNPhysicsVehicleWheel

The appearance and physical characteristics of an individual wheel associated with an physics vehicle behavior.

