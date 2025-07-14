

- QuickTime File Format
- Structuring movie data and features
- Creating an effect description
-  Required atoms of an effects description 

Article

# Required atoms of an effects description

Specify the required atoms for your effects description.

## Overview

There are several required atoms that an effect description must contain. The first is the `kParameterWhatName` atom. The `kParameterWhatName` atom contains the name of the effect. This specifies which of the available effects to use.

The code snippet shown in the following listing adds a `kParameterWhatName` atom to the atom container `effectDescription`. The constant `kCrossFadeTransitionType` contains the name of the cross-fade effect.

```
effectCode = kCrossFadeTransitionType;
QTInsertChild(effectDescription, kParentAtomIsContainer,
                kParameterWhatName, kParameterWhatID, 0,
                sizeof(effectCode), &effectCode, nil);
```

In addition to the `kParameterWhatName` atom, the effect description for an effect that uses sources must contain one or more `kEffectSourceName` atoms. Each of these atoms contains the name of one of the effect’s sources. An input map is used to map these names to the actual tracks of the movie that are the sources. Creating an input map describes how to create the input map.

## See Also

### Effect descriptions

Structure of an effect description

An effect description is the sole media sample for an effect track.

Parameter atoms of an effects description

Customize your effect with parameter atoms.

Creating an input map

Describe and name sources with an input map.

