

- Application Services
- Speech Synthesis Manager
-  PhonemeDescriptor 

Structure

# PhonemeDescriptor

Defines a phoneme descriptor structure.

macOS 10.0+

``` source
struct PhonemeDescriptor
```

## Overview

By calling the GetSpeechInfo function with the `soPhonemeSymbols` selector, you can obtain a phoneme descriptor structure, which describes all phonemes defined for the current synthesizer.

A common use for a phoneme descriptor structure is to provide a graphical display to the user of all available phonemes. Such a list is used only for a user entering phonemic data directly rather than just entering text.

## Topics

### Initializers

init()

init(phonemeCount: Int16, thePhonemes: PhonemeInfo)

### Instance Properties

var phonemeCount: Int16

The number of phonemes that the current synthesizer defines. Typically, this will correspond to the number of phonemes in the language supported by the synthesizer.

var thePhonemes: PhonemeInfo

An array of phoneme information structures.

