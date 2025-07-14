

- PHASE
-  Spatial Mixing 

API Collection

# Spatial Mixing

Define environmental characteristics that determine how sound plays in your app’s 3D soundscape.

## Overview

Spatial mixing refers to the process by which PHASE emits one or more simultaneous sounds in 3D space and layers in optional environmental effects. For a walkthrough that demonstrates spatial mixing, see Playing sound from a location in a 3D scene.

## Topics

### Setup

class PHASESpatialMixerDefinition

An audio-layering object that produces environmental effects and plays sound with a 3D position and orientation.

### Sound Reflections and Resonance

class PHASESpatialPipeline

An object that specifies the volume of optional environmental effects.

class PHASESpatialPipelineEntry

An audio layer with an adjustable volume for a spatial mixer’s output.

struct PHASESpatialCategory

Sound resonance effects for spatial mixing.

struct Flags

Sound resonance options for a spatial pipeline.

### Distance Modeling

class PHASEGeometricSpreadingDistanceModelParameters

An object that dissipates sound frequencies over distance.

class PHASEEnvelopeDistanceModelParameters

A graph of points and curves that shapes the volume of a sound over distance.

class PHASEDistanceModelFadeOutParameters

A distance over which the framework fades out sound.

class PHASEDistanceModelParameters

A base class for a sound’s rate of change over distance.

### Sound Directivity

class PHASECardioidDirectivityModelParameters

An object that directs sound in a heart-shaped curve surrounding a sound source.

class PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

class PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

class PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

class PHASEDirectivityModelParameters

A base class for objects that direct sound.

## See Also

### Audio Layering and Effects

class PHASEChannelMixerDefinition

An audio-layering object that routes sound directly to the device’s output.

class PHASEAmbientMixerDefinition

An audio-layering object that outputs sound in a particular direction in 3D space.

class PHASEMixerDefinition

An object to initialize a mixer with a given configuration.

class PHASEMixer

An object that combines multiple audio signals into a single signal.

class PHASEDefinition

A base class that adds a name to framework definitions.

