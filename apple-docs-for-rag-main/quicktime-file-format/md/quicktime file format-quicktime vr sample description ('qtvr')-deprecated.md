

- QuickTime File Format
-  QuickTime VR sample description ('qtvr') Deprecated

Atom

# QuickTime VR sample description ('qtvr')

Describe QuickTime VR samples.

Deprecated

VR Media is deprecated in the QuickTime file format. The information that follows documents existing content containing VR Media and should not be used for new development.

## Overview

Whereas the QuickTime VR media sample is simply the node information itself, all sample descriptions are required by QuickTime to have a certain structure for the first several bytes. The structure for the QuickTime VR sample description is as follows:

```
typedef struct QTVRSampleDescription {
    UInt32                              size;
    UInt32                              type;
    UInt32                              reserved1;
    UInt16                              reserved2;
    UInt16                              dataRefIndex;
    UInt32                              data;
} QTVRSampleDescription, *QTVRSampleDescriptionPtr, **QTVRSampleDescriptionHandle;
```

## Topics

### Data fields

size

The size, in bytes, of the sample description header structure.

type

The sample description type.

reserved1

Reserved.

reserved2

Reserved.

dataRefIndex

Reserved.

data

The VR world atom container.

