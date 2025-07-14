

- Application Services
- ColorSync Manager
-  Element Tags and Signatures for Version 1.0 Profiles 

# Element Tags and Signatures for Version 1.0 Profiles

Define tags and signatures used for version 1.0 profiles.

## Overview

The ICC version 2.x profile format differs from the version 1.0 profile format, and ColorSync Manager routines for updating a profile and searching for profiles do not work with version 1.0 profiles. However, your application can use version 1.0 profiles with all other ColorSync routines. For example, you can open a version 1.0 profile using the function CMOpenProfile, obtain the version 1.0 profile header using the function CMGetProfileHeader, and access version 1.0 profile elements using the function CMGetProfileElement.

To make this possible, the ColorSync Manager includes support for the version 1.0 profile header structure and synthesizes tags to allow you to access four 1.0 elements outside the version 1.0 profile header. This enumeration defines these tags.

## Topics

### Constants

var cmCS1ChromTag: Int

The tag signature for the profile chromaticities tag whose element data specifies the XYZ chromaticities for the six primary and secondary colors (red, green, blue, cyan, magenta, and yellow).

var cmCS1TRCTag: Int

The tag signature for profile tonal response curve data for the associated device.

var cmCS1NameTag: Int

The tag signature for the profile name string. This is an international string consisting of a Macintosh script code followed by a 63-byte text string identifying the profile.

var cmCS1CustTag: Int

Private data for a custom CMM.

