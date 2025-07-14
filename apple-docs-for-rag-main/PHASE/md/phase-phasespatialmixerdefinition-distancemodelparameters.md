

- PHASE
- PHASESpatialMixerDefinition
-  distanceModelParameters 

Instance Property

# distanceModelParameters

An effect that changes sound as it carries over a distance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var distanceModelParameters: PHASEDistanceModelParameters? { get set }
```

## Discussion

Similar to a Doppler effect, this property changes how an audio source sounds as its distance between the listener increases or decreases in 3D space. The available options are:

PHASEGeometricSpreadingDistanceModelParameters  
Create a realistic effect by dissipating certain frequency ranges of the audio spectrum differently with distance.

PHASEEnvelopeDistanceModelParameters  
Take full control of the sound’s volume by graphing its loudness using points and curves over the distance.

### Programmatically Check Sound Dissipation

After setting a value for this property, you can move a looping sound source to tweak the effect to your app’s particular requirements. The following code programmaticaly moves a looping source away from the listener along the z-axis:

- Swift
- Objective-C

```
spatialSamplerNode.playbackType = PHASEPlaybackType.looping
// ... 
var sourceTransform: PHASETransform3D = origin
sourceTransform.columns.3.z -= 6.0
while (true) {
    var posToSet: PHASETransform3D = source.transform
    posToSet.columns.3.z -= 0.05
    if (posToSet.columns.3.z 

```
spatialSamplerNode.playbackType = PHASEPlaybackTypeLooping;
// ...
PHASETransform3D sourceTransform = origin;
sourceTransform.columns[3].z -= 6.f;
while (1) {
    PHASETransform3D posToSet = _source.transform;
    posToSet.columns[3].z -= .05f;
    if (posToSet.columns[3].z 

```
```

