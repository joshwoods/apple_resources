

- Core Services
- Apple Events
-  AEKeyDesc 

Structure

# AEKeyDesc

Associates a keyword with a descriptor to form a keyword-specifieddescriptor.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AEKeyDesc
```

## Overview

The Apple Event Manager uniquely identifies the various partsof an Apple event by means of keywords associated with correspondingdescriptors. A keyword is an arbitrary constant of type AEKeyword that representsa four-character code.

## Topics

### Initializers

init()

init(descKey: AEKeyword, descContent: AEDesc)

### Instance Properties

var descContent: AEDesc

A descriptor of type AEDesc that stores the keyword descriptordata. See AEDesc.

var descKey: AEKeyword

A four-character code of type AEKeyword that uniquely identifies thekey that is associated with the data in the structure. Some keywordconstants are described in Keyword Attribute Constants and Keyword Parameter Constants.See AEKeyword.

