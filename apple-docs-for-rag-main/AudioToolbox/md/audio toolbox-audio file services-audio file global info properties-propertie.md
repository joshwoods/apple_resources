

- Audio Toolbox
- Audio File Services
-  Audio File Global Info Properties 

API Collection

# Audio File Global Info Properties

Access these properties using the functions described in Working with Global Information.

## Overview

A *specifier*, in the context of one of these properties, is a pointer to a buffer containing data specific to the property. Each property description names the type of the data required. You provide the data when accessing these properties using the functions described in Working with Global Information.

## Topics

### Constants

var kAudioFileGlobalInfo_ReadableTypes: AudioFilePropertyID

An array of `UInt32` values containing the file types (such as AIFF, WAVE, and so forth) that can be opened for reading.

var kAudioFileGlobalInfo_WritableTypes: AudioFilePropertyID

An array of `UInt32` values containing the file types (such as AIFF, WAVE, and so forth) that can be opened for writing.

var kAudioFileGlobalInfo_FileTypeName: AudioFilePropertyID

The name for the file type.

var kAudioFileGlobalInfo_AvailableFormatIDs: AudioFilePropertyID

An array of format IDs for formats that can be read.

var kAudioFileGlobalInfo_AvailableStreamDescriptionsForFormat: AudioFilePropertyID

An array of audio stream basic description structures, which contain all the formats for a particular file type and format ID.

var kAudioFileGlobalInfo_AllExtensions: AudioFilePropertyID

A `CFArray` of `CFStrings` containing all recognized file extensions. You can use this array when creating an `NSOpenPanel` (declared in the AppKit’s `NSOpenPanel.h` header file).

var kAudioFileGlobalInfo_AllHFSTypeCodes: AudioFilePropertyID

An array of HFS type codes containing all recognized HFS type codes. For more information on HFS type codes, see Audio Toolbox’s `ExtendedAudioFile.h` header file.

var kAudioFileGlobalInfo_AllUTIs: AudioFilePropertyID

A `CFArray` of `CFString` of all UTIs (Universal Type Identifiers) recognized by Audio File Services.

var kAudioFileGlobalInfo_AllMIMETypes: AudioFilePropertyID

A `CFArray` of CF strings of all MIME types are recognized by Audio File Services.

var kAudioFileGlobalInfo_ExtensionsForType: AudioFilePropertyID

A `CFArray` of CF strings containing the recognized file extensions for a specified type.

var kAudioFileGlobalInfo_HFSTypeCodesForType: AudioFilePropertyID

An array of HFS type codes corresponding to a specified file type. The first type in the array is the preferred one to use.

var kAudioFileGlobalInfo_UTIsForType: AudioFilePropertyID

A `CFArray` of `CFString` of all Universal Type Identifiers recognized by a specified file type.

var kAudioFileGlobalInfo_MIMETypesForType: AudioFilePropertyID

A `CFArray` of `CFString` of all MIME types recognized by a specified file type.

var kAudioFileGlobalInfo_TypesForExtension: AudioFilePropertyID

An array of all audio file type IDs that support a specified filename extension.

var kAudioFileGlobalInfo_TypesForHFSTypeCode: AudioFilePropertyID

An array of all audio file type IDs that support a specified `HFSTypeCode`.

var kAudioFileGlobalInfo_TypesForUTI: AudioFilePropertyID

An array of all audio file type IDs that support a specified UTI.

var kAudioFileGlobalInfo_TypesForMIMEType: AudioFilePropertyID

An array of all audio file type IDs that support a specified MIME type.

## See Also

### Constants

typealias AudioFileTypeID

Operating system constants that indicate the type of file to be written or a hint about what type of file to expect from data provided.

Audio File Creation Flags

Flags to set when creating an audio file.

enum AudioFilePermissions

Flags for use when opening an audio file.

Audio File Loop Direction Constants

The playback direction of a looped segment of an audio file.

Audio File Marker Types

A type of marker within a file used in the `mType` field of the AudioFileMarker structure.

struct AudioFileRegionFlags

Flags that specify a playback direction for an audio file region structure.

Audio File Packet Translation Flags

Flags specified in a packet translation structure.

Info String Keys

Key values of properties to get and set using Audio File Services functions and provide a common way to get the same information out of several different kinds of files.

Audio File Properties

Properties used by the functions described in getting and setting pieces of data in audio files. See Working with Global Information for details.

