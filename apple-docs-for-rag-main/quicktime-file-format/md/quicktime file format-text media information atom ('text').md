

- QuickTime File Format
-  Text media information atom ('text') 

Atom

# Text media information atom ('text')

An atom that contains information about text media.

## Mentioned in 

QuickTime File Format change log

## Overview

The text media also requires a text media information atom. This media information atom is stored in a base media information atom (`'minf'`) in the base media information header atom (`'gmhd'`) (see Base media information atom ('minf')). The type of the text media information atom is `'text'`.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this text media information atom.

Type

A 32-bit integer that identifies the atom type.

Matrix structure

A matrix structure associated with this text media.

## See Also

### Storing text data

Text sample description

An atom that defines how to interpret text media data.

Text sample data

An atom that contains text data.

Hypertext and wired text

Store hypertext in a text track sample atom.

