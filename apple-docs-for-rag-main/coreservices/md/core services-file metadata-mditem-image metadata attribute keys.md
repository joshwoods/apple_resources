

- Core Services
- File Metadata
- MDItem
-  Image Metadata Attribute Keys 

API Collection

# Image Metadata Attribute Keys

Metadata attribute keys that are common to image files.

## Topics

### Constants

let kMDItemPixelHeight: CFString!

The height, in pixels, of the contents. For example, the image height or the video frame height. A CFNumber.

let kMDItemPixelWidth: CFString!

The width, in pixels, of the contents. For example, the image width or the video frame width. A CFNumber.

let kMDItemPixelCount: CFString!

The total number of pixels in the contents. Same as kMDItemPixelWidth x kMDItemPixelHeight. A CFNumber.

let kMDItemColorSpace: CFString!

The color space model used by the document contents. For example, “RGB”, “CMYK”, “YUV”, or “YCbCr”. A CFString.

let kMDItemBitsPerSample: CFString!

The number of bits per sample. For example, the bit depth of an image (8-bit, 16-bit etc...) or the bit depth per audio sample of uncompressed audio data (8, 16, 24, 32, 64, etc..). A CFNumber.

let kMDItemFlashOnOff: CFString!

Indicates if a camera flash was used. A CFNumber.

let kMDItemFocalLength: CFString!

The actual focal length of the lens, in millimeters. A CFNumber.

let kMDItemAcquisitionMake: CFString!

The manufacturer of the device used to aquire the document contents. A CFString.

let kMDItemAcquisitionModel: CFString!

The model of the device used to aquire the document contents. For example, 100, 200, 400, etc. A CFString.

let kMDItemISOSpeed: CFString!

The ISO speed used to acquire the document contents. A CFNumber.

let kMDItemOrientation: CFString!

The orientation of the document contents. Possible values are 0 (landscape) and 1 (portrait). A CFNumber.

let kMDItemLayerNames: CFString!

The names of the layers in the file. A CFArray of CFStrings.

let kMDItemWhiteBalance: CFString!

The white balance setting used to acquire the document contents. Possible values are 0 (auto white balance) and 1 (manual). A CFNumber.

let kMDItemAperture: CFString!

The aperture setting used to acquire the document contents. This unit is the APEX value. A CFNumber.

let kMDItemProfileName: CFString!

The name of the color profile used by the document contents. A CFString.

let kMDItemResolutionWidthDPI: CFString!

Resolution width, in DPI, of this image. A CFNumber.

let kMDItemResolutionHeightDPI: CFString!

Resolution height, in DPI, of this image. A CFNumber.

let kMDItemExposureMode: CFString!

The exposure mode used to acquire the document contents. A CFNumber.

let kMDItemExposureTimeSeconds: CFString!

The exposure time, in seconds, used to acquire the document contents. A CFNumber.

let kMDItemEXIFVersion: CFString!

The version of the EXIF header used to generate the metadata. A CFString.

let kMDItemAlbum: CFString!

The title for a collection of media. This is analagous to a record album, or photo album. A CFString.

let kMDItemHasAlphaChannel: CFString!

Indicates if this image file has an alpha channel. A CFBoolean.

let kMDItemRedEyeOnOff: CFString!

Indicates if red-eye reduction was used to take the picture. A CFBoolean.

let kMDItemMeteringMode: CFString!

The metering mode used to take the image. A CFString.

let kMDItemMaxAperture: CFString!

The smallest f-number of the lens. Ordinarily it is given in the range of 00.00 to 99.99. A CFNumber.

let kMDItemFNumber: CFString!

The diameter of the diaphragm aperture in terms of the effective focal length of the lens.

let kMDItemExposureProgram: CFString!

The class of the exposure program used by the camera to set exposure when the image is taken. Possible values include: Manual, Normal, and Aperture priority. A CFString.

let kMDItemExposureTimeString: CFString!

The time of the exposure. A CFString.

let kMDItemEXIFGPSVersion: CFString!

The version of GPSInfoIFD in EXIF used to generate the metadata. A CFString.

let kMDItemAltitude: CFString!

The altitude of the item in meters above sea level, expressed using the WGS84 datum. Negative values lie below sea level. A CFString.

let kMDItemLatitude: CFString!

The latitude of the item in degrees north of the equator, expressed using the WGS84 datum. Negative values lie south of the equator. A CFString.

let kMDItemLongitude: CFString!

The longitude of the item in degrees east of the prime meridian, expressed using the WGS84 datum. Negative values lie west of the prime meridian. A CFString.

let kMDItemTimestamp: CFString!

The timestamp on the item. This generally is used to indicate the time at which the event captured by the item took place. A CFString.

let kMDItemSpeed: CFString!

The speed of the item, in kilometers per hour. A CFString.

let kMDItemGPSTrack: CFString!

The direction of travel of the item, in degrees from true north. A CFString.

let kMDItemImageDirection: CFString!

The direction of the item's image, in degrees from true north. A CFString.

let kMDItemNamedLocation: CFString!

The name of the location or point of interest associated with the item. The name may be user provided. A CFString.

