

- Image I/O
-  IPTC Dictionary Keys 

API Collection

# IPTC Dictionary Keys

Metadata keys for International Press Telecommunications Council (IPTC) data.

## Overview

IPTC constants are metadata elements of the Information Interchange Model (IIM) used to provide information about images. The IIM was developed by the Newspaper Association of America (NAA) and the IPTC.

## Topics

### Dictionary

let kCGImagePropertyIPTCDictionary: CFString

A dictionary of key-value pairs for an image that uses International Press Telecommunications Council (IPTC) metadata.

### Image Categorization

let kCGImagePropertyIPTCUrgency: CFString

The urgency level.

let kCGImagePropertyIPTCSubjectReference: CFString

The subject.

let kCGImagePropertyIPTCCategory: CFString

The category.

let kCGImagePropertyIPTCSupplementalCategory: CFString

A supplemental category.

let kCGImagePropertyIPTCFixtureIdentifier: CFString

A fixture identifier.

let kCGImagePropertyIPTCKeywords: CFString

Keywords relevant to the image.

let kCGImagePropertyIPTCContentLocationCode: CFString

The content location code.

let kCGImagePropertyIPTCContentLocationName: CFString

The content location name.

let kCGImagePropertyIPTCEditStatus: CFString

The edit status.

let kCGImagePropertyIPTCEditorialUpdate: CFString

An editorial update.

let kCGImagePropertyIPTCObjectCycle: CFString

The editorial cycle (morning, evening, or both) of the image.

### Image Information

let kCGImagePropertyIPTCImageType: CFString

The image type.

let kCGImagePropertyIPTCImageOrientation: CFString

The image orientation (portrait, landscape, or square).

let kCGImagePropertyIPTCLanguageIdentifier: CFString

The language identifier, a two-letter code defined by ISO 639:1988.

let kCGImagePropertyIPTCCaptionAbstract: CFString

The description of the image.

let kCGImagePropertyIPTCHeadline: CFString

A summary of the contents of the image.

let kCGImagePropertyIPTCCredit: CFString

The name of the service that provided the image.

let kCGImagePropertyIPTCStarRating: CFString

The star rating.

let kCGImagePropertyIPTCScene: CFString

The scene codes for the image; a scene code is a six-digit string.

### Copyright

let kCGImagePropertyIPTCCopyrightNotice: CFString

The copyright notice.

let kCGImagePropertyIPTCRightsUsageTerms: CFString

The usage rights for the image.

### Release Information

let kCGImagePropertyIPTCReleaseDate: CFString

The earliest day on which you can use the image, in the form CCYYMMDD.

let kCGImagePropertyIPTCReleaseTime: CFString

The earliest time at which you can use the image, in the form HHMMSS.

let kCGImagePropertyIPTCExpirationDate: CFString

The latest date you can use the image, in the form CCYYMMDD.

let kCGImagePropertyIPTCExpirationTime: CFString

The latest time on the expiration date you can use the image, in the form HHMMSS.

let kCGImagePropertyIPTCSpecialInstructions: CFString

Special instructions about the use of the image.

let kCGImagePropertyIPTCActionAdvised: CFString

The advised action.

let kCGImagePropertyIPTCReferenceService: CFString

The reference service.

let kCGImagePropertyIPTCReferenceDate: CFString

The reference date.

let kCGImagePropertyIPTCReferenceNumber: CFString

The reference number.

let kCGImagePropertyIPTCDateCreated: CFString

The creation date.

let kCGImagePropertyIPTCTimeCreated: CFString

The creation time.

let kCGImagePropertyIPTCDigitalCreationDate: CFString

The digital creation date.

let kCGImagePropertyIPTCDigitalCreationTime: CFString

The digital creation time.

### Personnel

let kCGImagePropertyIPTCByline: CFString

The name of the person who created the image.

let kCGImagePropertyIPTCBylineTitle: CFString

The title of the person who created the image.

let kCGImagePropertyIPTCSource: CFString

The original owner of the image.

let kCGImagePropertyIPTCContact: CFString

The contact information for getting details about the image.

let kCGImagePropertyIPTCWriterEditor: CFString

The name of the person who wrote or edited the description of the image.

let kCGImagePropertyIPTCCreatorContactInfo: CFString

The creator’s contact info.

IPTC Creator Contact Info Dictionary Keys

Keys for an image that uses International Press Telecommunications Council (IPTC) metadata.

### Location Data

let kCGImagePropertyIPTCCity: CFString

The city where the image was created.

let kCGImagePropertyIPTCSubLocation: CFString

The location within the city where the image was created.

let kCGImagePropertyIPTCProvinceState: CFString

The province or state.

let kCGImagePropertyIPTCCountryPrimaryLocationCode: CFString

The primary country code, a three-letter code defined by ISO 3166-1.

let kCGImagePropertyIPTCCountryPrimaryLocationName: CFString

The primary country name.

let kCGImagePropertyIPTCOriginalTransmissionReference: CFString

The call letter or number combination associated with the originating point of an image.

### Software Program

let kCGImagePropertyIPTCOriginatingProgram: CFString

The originating application.

let kCGImagePropertyIPTCProgramVersion: CFString

The application version.

### Object Details

let kCGImagePropertyIPTCObjectTypeReference: CFString

The object type.

let kCGImagePropertyIPTCObjectAttributeReference: CFString

The object attribute.

let kCGImagePropertyIPTCObjectName: CFString

The object name.

### IPTC Extension

let kCGImageMetadataNamespaceIPTCExtension: CFString

let kCGImageMetadataPrefixIPTCExtension: CFString

## See Also

### Common Image Properties

Image Properties

Properties that apply to the container in general, and not necessarily to an individual image in the container.

EXIF Dictionary Keys

Metadata keys for Exchangeable Image File Format (EXIF) data.

GPS Dictionary Keys

Keys for Global Positioning System (GPS) information.

WebP Data

Metadata keys for WebP metadata.

