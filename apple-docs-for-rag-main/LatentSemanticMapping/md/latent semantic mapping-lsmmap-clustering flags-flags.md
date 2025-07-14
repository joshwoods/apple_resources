

- Latent Semantic Mapping
- LSMMap
-  Clustering Flags 

API Collection

# Clustering Flags

Options for creating clusters.

## Overview

Specify these options for LSMMapCreateClusters(_:_:_:_:_:).

## Topics

### Constants

var kLSMClusterCategories: Int

An option that specifies to cluster categories.

var kLSMClusterWords: Int

An option that specifies to cluster words.

var kLSMClusterTokens: Int

An option that specifies to cluster binary tokens.

var kLSMClusterKMeans: Int

An option that specifies to cluster using a k-means algorithm.

var kLSMClusterAgglomerative: Int

An option that specifies to cluster using an agglomerative algorithm.

## See Also

### Starting Classification Mode

func LSMMapCompile(LSMMap) -> OSStatus

Compiles the map into executable form and puts it into mapping mode, preparing it for the classification of texts.

func LSMMapCreateClusters(CFAllocator?, LSMMap, CFArray?, CFIndex, CFOptionFlags) -> Unmanaged&lt;CFArray>?

Computes a set of clusters that group similar categories or words.

func LSMMapApplyClusters(LSMMap, CFArray) -> OSStatus

Groups categories or words (tokens) into the specified sets of clusters.

