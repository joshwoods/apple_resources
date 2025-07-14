

- QuickTime File Format
- Structuring movie data and features
-  Creating an effect description 

# Creating an effect description

Tell QuickTime which effect to execute and control how the effect behaves at runtime with an effect description.

## Overview

An effect description tells QuickTime which effect to execute and contains the parameters that control how the effect behaves at runtime. You create an effect description by creating an atom container, inserting a QT atom that specifies the effect, and inserting a set of QT atoms that set its parameters.

There are support functions you can call to assist you in this process. `QTCreateStandardParameterDialog` returns a complete effect description that you can use, including user-selected settings; you only need to add `kEffectSourceName` atoms to the description for effects that require sources. At a lower level, `QTGetEffectsList` returns a list of the available effects and `ImageCodecGetParameterList` will return a description of the parameters for an effect, including the default value for each parameter in the form of a QT atom that can be inserted directly into an effect description.

## Topics

### Effect descriptions

Structure of an effect description

An effect description is the sole media sample for an effect track.

Required atoms of an effects description

Specify the required atoms for your effects description.

Parameter atoms of an effects description

Customize your effect with parameter atoms.

Creating an input map

Describe and name sources with an input map.

## See Also

### Movie features

Preparing sound and subtitle alternate groups for use with Apple devices

Create collections of tracks that all serve the same purpose, where any track in the group can be substituted for another in a movie.

