

- Application Services
- Speech Synthesis Manager
-  PhonemeInfo 

Structure

# PhonemeInfo

Defines a structure that stores information about a phoneme.

macOS 10.0+

``` source
struct PhonemeInfo
```

## Overview

Ordinarily, you use a phoneme information structure to show the user how to enter text to represent a particular phoneme when the `'PHON'` input mode is activated.

You might use the information contained in the `hiliteStart` and `hiliteEnd` fields to highlight the characters in the example word that represent the phoneme.

To obtain a phoneme information structure for an individual phoneme, you must obtain a list of phonemes through a phoneme descriptor structure.

## Topics

### Initializers

init()

init(opcode: Int16, phStr: Str15, exampleStr: Str31, hiliteStart: Int16, hiliteEnd: Int16)

### Instance Properties

var exampleStr: Str31

An example word that illustrates use of the phoneme.

var hiliteEnd: Int16

The number of characters between the beginning of the example word and the end of the portion of that word representing the phoneme.

var hiliteStart: Int16

The number of characters in the example word that precede the portion of that word representing the phoneme.

var opcode: Int16

The opcode for the phoneme.

var phStr: Str15

The string used to represent the phoneme. The string does not necessarily have a phonetic connection to the phoneme, but might simply be an abstract textual representation of it.

