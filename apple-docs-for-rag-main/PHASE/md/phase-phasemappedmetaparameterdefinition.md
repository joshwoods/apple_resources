

- PHASE
-  PHASEMappedMetaParameterDefinition 

Class

# PHASEMappedMetaParameterDefinition

A metaparameter that graphs an input value on a set of mathematical curves.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMappedMetaParameterDefinition
```

## Overview

This class takes a metaparameter as input and plots its value on a curve defined by the envelope property.

Whereas the envelope’s function in PHASEBlendNodeDefinition and PHASEEnvelopeDistanceModelParameters takes time because the relevant audio starts as its input parameter, in the case of the envelope property for this class, the app has full control over the input metaparameter’s value.

## Topics

### Creating a Mapped Metaparameter

init(inputMetaParameterDefinition: PHASENumberMetaParameterDefinition, envelope: PHASEEnvelope)

Creates a specification for a metaparameter that the app plots on a graph defined by the given set of curves.

convenience init(inputMetaParameterDefinition: PHASENumberMetaParameterDefinition, envelope: PHASEEnvelope, identifier: String)

Creates a specification for a named metaparameter that the app plots on a graph defined by the given set of curves.

### Inspecting the Input Parameter

var inputMetaParameterDefinition: PHASENumberMetaParameterDefinition

A linear input value to plot on a curve.

### Inspecting the Envelope

var envelope: PHASEEnvelope

A collection of line segments that curve and connect to form a graph.

## Relationships

### Inherits From

- PHASENumberMetaParameterDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

