

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  cmProfileError 

Global Variable

# cmProfileError

There is something wrong with the content of the profile

Mac Catalyst 13.0+macOS 10.0+

``` source
var cmProfileError: Int { get }
```

## See Also

### Result Codes

var cmMethodError: Int

An error occurred during the CMM arbitration process that determines the CMM to use

var cmMethodNotFound: Int

CMM not present

var cmProfileNotFound: Int

Responder error

var cmProfilesIdentical: Int

Profiles are the same

var cmCantConcatenateError: Int

Profiles cannot be concatenated

var cmCantXYZ: Int

CMM does not handle XYZ color space

var cmCantDeleteProfile: Int

Responder error

var cmUnsupportedDataType: Int

Responder error

var cmNoCurrentProfile: Int

Responder error

var cmElementTagNotFound: Int

The tag you specified is not in the specified profile

var cmIndexRangeErr: Int

Tag index out of range

var cmCantDeleteElement: Int

Cannot delete the specified profile element

var cmFatalProfileErr: Int

Returned from File Manager while updating a profile file in response to `CMUpdateProfile`; profile content may be corrupted

var cmInvalidProfile: Int

Profile reference is invalid or refers to an inappropriate profile

var cmInvalidProfileLocation: Int

Operation not supported for this profile location

var cmInvalidSearch: Int

Bad search handle

var cmSearchError: Int

Internal error occurred during profile search

var cmErrIncompatibleProfile: Int

Unspecified profile error

var cmInvalidColorSpace: Int

Profile color space does not match bitmap type

var cmInvalidSrcMap: Int

Source pixel map or bitmap was invalid

var cmInvalidDstMap: Int

Destination pix/bit map was invalid

var cmNoGDevicesError: Int

Begin matching or end matching—no graphics devices available

var cmInvalidProfileComment: Int

Bad profile comment during `drawpicture`

var cmRangeOverFlow: Int

One or more output color value overflows in color conversion; all input color values will be converted and the overflow will be clipped

var cmCantCopyModifiedV1Profile: Int

It is illegal to copy version 1.0 profiles that have been modified

var cmNamedColorNotFound: Int

The specified named color was not found in the specified profile

var cmCantGamutCheckError: Int

Gamut checking not supported by this color world—that is, the color world does not contain a gamut table because it was built with gamut checking turned off

var cmDeviceDBNotFoundErr: Int

Preferences not found or loaded; returned by a CM device integration routine.

var cmDeviceAlreadyRegistered: Int

Device already registered; returned by a CM device integration routine.

var cmDeviceNotRegistered: Int

Device not found; returned by a CM device integration routine.

var cmDeviceProfilesNotFound: Int

Profiles not found; returned by a CM device integration routine.

var cmInternalCFErr: Int

CoreFoundation failure; returned by a CM device integration routine.

