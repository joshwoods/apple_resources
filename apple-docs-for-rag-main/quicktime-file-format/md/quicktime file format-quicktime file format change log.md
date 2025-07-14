

- QuickTime File Format
-  QuickTime File Format change log 

Article

# QuickTime File Format change log

Changes to the QuickTime File Format.

## Overview

### 2016-09-13

#### Updated

- Updated the color atom (`'colr'`) to include information on new color standards, including DCI P3, P3 D65, and ITU-R BT.2020.

### 2015-02-14

#### Added

- A new facility for timed metadata tracks has been incorporated, see Timed metadata media. Introduce `'cdsc'` track reference type, see Track reference type atom. Added more well-known metadata data types, see Type indicator.

### 2014-02-11

#### Updated

- Updated the section on closed caption tracks.

### 2012-08-14

#### Updated

- Corrected the values for `kQTSampleDependency_OtherSamplesDependOnThisSample` and `kQTSampleDependency_-NoOtherSampleDependsOnThisSample`.

### 2012-08-01

#### Added

- Added Track exclude from autoselection atom ('txas').

- Added `clcp`, `fall`, `folw`, and `forc` to Track reference type atom.

- Added Text media information atom ('text'), Closed captioning media, and Subtitle media.

- Added Preparing sound and subtitle alternate groups for use with Apple devices.

#### Updated

- In User data atoms, expanded the description of `'tnam'` and added `'tagc'` with related section Media Characteristic Tags.

- Explained alternate groups in Alternate group.

- Corrected structure of `gmhd` and `gmin` in Base media information atom ('minf').

- General Structure of a Sample Description in Sample description atom ('stsd') includes emphasized importance of data size due to occasional terminating zeroes.

- Timecode media information atom ('tcmi') now documents the reserved integer after the text size.

- “Audio track” changed to “sound track” for consistency.

#### Deprecated

- Deprecated `‘rsrc’` data reference.

### 2011-07-13

#### Added

- The sound sample description v2 format along with the definition of two new sound sample description extensions, see Sound sample description version 2 ('stsd').

- New atoms for the display of track aperture in different modes, see Track aperture mode dimensions atom ('tapt').

- New sample atoms for handling out-of-order movie samples, see Sample atoms.

- Audio priming-handling encoder delay in AAC, which treats how to handle temporal positioning of AAC audio data explicitly.

#### Updated

- The Macintosh language codes table has been updated with current language names, see Language code values and the related Extended language tag atom ('elng') defined.

### 2010-08-03

#### Updated

- Corrected the order of fields described in the Metadata handler atom ('hdlr') structure.

### 2010-05-03

#### Added

- Added description of clip-based metadata and specific key/value pairs for location metadata.

### 2007-09-04

#### Added

- First public release of complete, updated *QuickTime File Format Specification* with information about atoms and atom types.

- Added licensing information and disclaimer for developers.

- A QuickTime file may now contain a file type compatibility atom. See File type compatibility atom ('ftyp').

- A movie atom may now contain a movie profile atom. See Movie profile atom ('prfl').

- A track atom may now contain a track profile atom. See Track profile atom ('prfl').

- Video sample descriptions may now contain a pixel aspect ratio atom for non-square pixels. See Pixel aspect ratio ('pasp') (`'pasp'`).

- Video sample descriptions may now also contain a color parameter atom. See Color parameter atom ('colr') (`'colr'`).

- Video sample descriptions may now a clean aperture atom. See Clean aperture ('clap') (`'clap'`).

- MPEG-4 video and audio sample descriptions may now contain elementary stream descriptor atoms. See MPEG-4 elementary stream descriptor atom ('esds') (`'esds'`) and MPEG-4 elementary stream descriptor atom ('esds') (`'esds'`).

#### Updated

- Modified introductory sections and atom descriptions; updated artwork and edited for technical accuracy.

- The sound description record has been expanded to represent variable bit-rate compression more accurately. See Sound sample descriptions.

- The section describing MPEG-4 audio has been modified. See MPEG-4 Audio in Sound sample data.

- It is now recommended that the file creation and modification times be set using UTC, rather than local time zones. See Calendar date and time values.

- User data text may now be encoded using either Macintosh text encoding or ISO text encoding (Unicode). See User Data Text Strings and Language Codes in User data atoms.

- It is now possible to specify languages using either Macintosh language codes or ISO language codes. See Language code values.

