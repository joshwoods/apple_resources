

- Kernel
- Kernel Data Types
-  mbuf_stat 

# mbuf_stat

macOS 10.6+

``` source
struct mbuf_stat {
    ...
};
```

## Discussion

The mbuf_stat contains mbuf statistics.

## Topics

### Fields

mbufs

Number of mbufs (free or otherwise).

clusters

Number of clusters (free or otherwise).

clfree

Number of free clusters.

drops

Number of times allocation failed.

wait

Number of times allocation blocked.

drain

Number of times protocol drain functions were called.

mtypes

An array of counts of each type of mbuf allocated.

mcfail

Number of times m_copym failed.

mpfail

Number of times m_pullup failed.

msize

Length of an mbuf.

mclbytes

Length of an mbuf cluster.

minclsize

Minimum length of data to allocate a cluster. Anything smaller than this should be placed in chained mbufs.

mlen

Length of data in an mbuf.

mhlen

Length of data in an mbuf with a packet header.

bigclusters

Number of big clusters.

bigclfree

Number of unused big clusters.

bigmclbytes

Length of a big mbuf cluster.

