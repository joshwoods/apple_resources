

- WebKit JS
-  WebKitCSSKeyframesRule 

# WebKitCSSKeyframesRule

`WebKitCSSKeyframesRule` objects represent the keyframes for a single animation, that is, the contents of an @-webkit-keyframes CSS rule used in animations. The WebKitAnimationEvent class encapsulate information about running animations.

## Topics

### Accessing Properties

name

The name of the target animation that is set using the -webkit-animation-name property.

cssRules

The set of style rules that define the keyframes following the animation name.

### Changing Rules

insertRule

Adds a keyframe rule to the collection of keyframes.

deleteRule

Removes a keyframe rule from the collection of keyframes.

findRule

Returns the keyframe rule for the specified selector.

