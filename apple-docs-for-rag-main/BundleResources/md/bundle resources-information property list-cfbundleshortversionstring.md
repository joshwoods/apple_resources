

- Bundle Resources
- Information Property List
-  CFBundleShortVersionString 

Property List Key

# CFBundleShortVersionString

The release or version number of the bundle.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Name  
Bundle versions string, short

Type  

string

## Discussion

This key is a user-visible string for the version of the bundle. The required format is three period-separated integers, such as 10.14.1. The string can only contain numeric characters (0-9) and periods.

Each integer provides information about the release in the format \[*Major*\].\[*Minor*\].\[*Patch*\]:

- Major: A major revision number.

- Minor: A minor revision number.

- Patch: A maintenance release number.

This key is used throughout the system to identify the version of the bundle.

## See Also

### Bundle version

CFBundleVersion

The version of the build that identifies an iteration of the bundle.

**Name:** Bundle version

CFBundleInfoDictionaryVersion

The current version of the Information Property List structure.

**Name:** InfoDictionary version

NSHumanReadableCopyright

A human-readable copyright notice for the bundle.

**Name:** Copyright (human-readable)

