

- Core Services
- File Metadata
- MDSchema
-  Available Metadata Attribute Keys 

API Collection

# Available Metadata Attribute Keys

Specify the available metadata attribute keys for a contenttype.

## Overview

These keys are in the dictionary returned by the function `MDSchemaCopyAttributesForContentType`.

## Topics

### Constants

let kMDAttributeDisplayValues: CFString!

An array of strings containing the availabledisplay metadata attribute keys, or `NULL` ifthe type is not known by the system.

let kMDAttributeAllValues: CFString!

An array of strings containing the availablemetadata attribute keys, or `NULL` ifthe type is not known by the system.

let kMDAttributeReadOnlyValues: CFString!

An array of strings containing the read-onlymetadata attribute keys, or `NULL` ifthe type is not known by the system.

let kMDExporterAvaliable: CFString!

A CFBoolean that indicates if an exporter is available for this UTI type.

