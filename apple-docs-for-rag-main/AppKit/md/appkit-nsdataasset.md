

- AppKit
-  NSDataAsset 

Class

# NSDataAsset

An object from a data set type stored in an asset catalog.

macOS 10.11+

``` source
class NSDataAsset
```

## Overview

The object’s content is stored as a set of one or more files with associated device attributes. These sets can also be tagged for use as on-demand resources.

### Initialize data assets

Data assets are initialized from a named data set in an asset catalog. You create data sets during app development. Each data set contains one or more data files. Each file has associated attributes for features of the device, including the minimum amount of memory and the version of Metal. When you initialize the data asset, the system selects the data file that best matches the current device.

For more information on the data set type in an asset catalog, see Data Set Type in Asset Catalog Format Reference. For information on asset catalogs, see Managing assets with asset catalogs.

### Access the data

You access the data file by using the data property. Because the property is of type NSData it provides methods for accessing the raw data only as bytes and ranges of bytes.

To access structured data, convert the bytes into the appropriate format. The system can convert some data types for you. One example is XML data using the init(data:) method of XMLParser. Other data types require code for parsing and converting the raw data. You may need to convert larger data files incrementally.

## Topics

### Initializing the data asset

convenience init?(name: NSDataAsset.Name)

Initializes and returns an object with a reference to the named data asset in an asset catalog.

init?(name: NSDataAsset.Name, bundle: Bundle)

Initializes and returns an object with a reference to the named data asset that’s in an asset catalog in the specified bundle.

### Accessing data

var data: Data

The raw data values in the data asset.

### Getting data asset information

var name: NSDataAsset.Name

The name of the data set in the asset catalog.

typealias Name

The name of a data asset.

var typeIdentifier: String

The uniform type identifier for the data asset.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

