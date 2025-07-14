

- QuickTime File Format
-  Storing and sharing media with QuickTime files 

# Storing and sharing media with QuickTime files

Build QuickTime files with atoms, QT atoms, and atom containers.

## Overview

Store QuickTime movies on disk using two basic structures for storing information: atoms (also known as simple atoms or classic atoms) and QT atoms. To understand how QuickTime movies are stored, you need to understand the basic atom structures. Most atoms that you encounter in the QuickTime File Format are simple or classic atoms. Both simple atoms and QT atoms, however, allow you to construct arbitrarily complex hierarchical data structures. Both also allow your application to ignore data that they don’t understand.

## Media description

A QuickTime file stores the description of its media separately from the media data.

The description is called the movie resource, movie atom, or simply the movie, and contains information such as the number of tracks, the video compression format, and timing information. The movie resource also contains an index describing where all the media data is stored.

The media data is the actual sample data, such as video frames and audio samples, used in the movie. The media data may be stored in the same file as the QuickTime movie, in a separate file, in multiple files, in alternate sources such as databases or real-time streams, or in some combination of these.

## Topics

### Building in QuickTime

Atoms

The basic data unit in a QuickTime file is the atom.

QT atoms and atom containers

An enhanced data structure that provide a more general-purpose storage format.

Creating, copying, and disposing of atom containers

Manage atoms in atom containers.

QuickTime movie files

The QuickTime file format describes the characteristics of QuickTime movie files.

