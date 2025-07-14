

- QuickTime File Format
- Deprecated atoms
- QuickTime VR file format
- Optimizing QuickTime VR movies for web playback
-  Sample atom container for the QTVR flattener 

Article

# Sample atom container for the QTVR flattener

Specify an import preview file for the flattener with atoms.

## Overview

The sample code in the following listing creates an atom container and adds atoms to indicate an import preview file for the flattener to use.

```
Boolean yes = true;
QTAtomContainer exportData;
QTAtom parent;
err = QTNewAtomContainer(&exportData);
// create a parent for the other settings atoms
err = QTInsertChild (exportData, kParentAtomIsContainer,
            QTVRFlattenerParentAtomType, 1, 0, 0, nil, &parent);
// Add child atom to indicate we want to import the preview from  a file
err = QTInsertChild (exportData, parent, QTVRImportPreviewAtomType,  1, 0,
            sizeof (yes), &yes, nil);
// Add child atom to tell which file to import
err = QTInsertChild (exportData, parent, QTVRImportSpecAtomType,  1, 0,
            sizeof (previewSpec), &previewSpec, nil);
// Tell the export component
MovieExportSetSettingsFromAtomContainer (qtvrExport, exportData);
```

Overriding the compression settings is a bit more complicated. You need to open a standard image compression dialog component and make calls to obtain an atom container that you can then pass to the QTVR Flattener component.

```
ComponentInstance sc;
QTAtomContainer compressorData;
SCSpatialSettings ss;
sc = OpenDefaultComponent(StandardCompressionType,StandardCompressionSubType);
ss.codecType = kCinepakCodecType;
ss.codec = nil;
ss.depth = 0;
ss.spatialQuality = codecHighQuality
err = SCSetInfo(sc, scSpatialSettingsType, &ss);
err = SCGetSettingsAsAtomContainer(sc, &compressorData);
MovieExportSetSettingsFromAtomContainer (qtvrExport, compressorData);
```

## See Also

### Optimizations

The QTVR flattener

Optimize a movie for delivery over the web.

