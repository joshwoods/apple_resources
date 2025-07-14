

- Audio Toolbox
-  kAudioFileGlobalInfo_AllMIMETypes 

Global Variable

# kAudioFileGlobalInfo_AllMIMETypes

A `CFArray` of CF strings of all MIME types are recognized by Audio File Services.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioFileGlobalInfo_AllMIMETypes: AudioFilePropertyID { get }
```

## Discussion

If you access this property, your app is responsible for releasing the CFArray object.

When accessing this property’s value, you must set the `inSpecifier` parameter to `NULL`.

## See Also

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

