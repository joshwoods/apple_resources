

- MediaExtension
-  MEFormatReader 

Protocol

# MEFormatReader

A protocol that defines the requirements for a format reader, which represents a single media asset.

macOS 14.0+

``` source
protocol MEFormatReader : NSObjectProtocol
```

## Overview

This protocol provides an interface for the Media Toolbox to interact with extension plug-in format readers, which provide information about media assets. `MEFormatReader` objects are always instantiated by the Media Toolbox.

Note

Developers who wish to build MediaExtension format readers using this API need to include a Format reader entitlement, provisioning profile, and specialized dictionary in their Info.plist file when building their extensions.

For more information, see Entitlements, Create a development provisioning profile, and Format reader property list dictionaries.

To create an `MEFormatReader` object, Media Toolbox first creates a primary MEByteSource object from a source media asset. It then creates an MEFormatReaderExtension object and calls its formatReader(with:options:) method.

Once a user installs and runs the host app, embedded MediaExtension format reader extensions become available to any app on the user’s system that opts in to using them by calling MTRegisterProfessionalVideoWorkflowFormatReaders().

Important

`MEFormatReader` objects run in a sandboxed process with restricted access to the filesystem, network, and other kernel resources.

## Topics

### Reading and parsing media assets

func loadFileInfo(completionHandler: (MEFileInfo?, (any Error)?) -> Void)

Loads the file info object with the properties of the media asset.

**Required**

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset.

**Required**

func loadTrackReaders(completionHandler: ([any METrackReader]?, (any Error)?) -> Void)

Loads the array of track readers that represent the tracks in the media asset.

**Required**

func parseAdditionalFragments(completionHandler: (MEFormatReaderParseAdditionalFragmentsStatus, (any Error)?) -> Void)

Incorporates additional fragments that the file received after the last time the format reader parsed it.

struct MEFormatReaderParseAdditionalFragmentsStatus

Informational status flags that the format reader returns after parsing additional fragments.

### Extension requirements

Format reader property list dictionaries

Include property list dictionaries to describe a format reader and register the formats it supports.

Format reader entitlement

Include an entitlement to indicate your extension is a MediaExtension format reader.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Format readers

protocol MEFormatReaderExtension

A protocol that defines a factory to create a new format reader with a byte source.

class MEFormatReaderInstantiationOptions

An object that contains options to pass to a format reader extension.

class MEFileInfo

An object that contains file properties from the media asset.

Format reader property list dictionaries

Include property list dictionaries to describe a format reader and register the formats it supports.

Format reader entitlement

Include an entitlement to indicate your extension is a MediaExtension format reader.

