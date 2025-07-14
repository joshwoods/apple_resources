

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 2D Real FFT 

API Collection

# Out-of-Place Functions for 2D Real FFT

Perform fast Fourier transforms out of place on 2D real data.

## Overview

The functions in this group use the following operation for a forward real-to-complex transform:

```
N0 = 1 realp[j1*IA1 + j0*IA0]
              + i * A->imagp[j1*IA1 + j0*IA0];
    h[j1][2*j0+1] = A->realp[j1*IA1 + j0*IA0]
              + i * A->imagp[j1*IA1 + j0*IA0];
}

// Perform Discrete Fourier Transform.
for (k1 = 0; k1 realp[0*IC1][0*IC0] = H[0   ][0   ].
C->imagp[0*IC1][0*IC0] = H[0   ][N0/2]
C->realp[1*IC1][0*IC0] = H[N1/2][0   ].
C->imagp[1*IC1][0*IC0] = H[N1/2][N0/2]

// Pack two vectors into output matrix "vertically":
// (This awkward format is due to a legacy implementation.)
for (k1 = 1; k1 realp[(2*k1+0)*IC1][0*IC0] = Re(H[k1][0   ]);
    C->realp[(2*k1+1)*IC1][0*IC0] = Im(H[k1][0   ]);
    C->imagp[(2*k1+0)*IC1][0*IC0] = Re(H[k1][N0/2]);
    C->imagp[(2*k1+1)*IC1][0*IC0] = Im(H[k1][N0/2]);
}

// Store regular elements:
for (k1 = 0; k1 realp[k1*IC1 + k0*IC0] = Re(H[k1][k0]);
    C->imagp[k1*IC1 + k0*IC0] = Im(H[k1][k0]);
}

```

The functions in this group use the following operation for an inverse complex-to-real transform:

```
N0 = 1 realp[0*IA1][0*IA0];
h[0   ][N0/2] = A->imagp[0*IA1][0*IA0];
h[N1/2][0   ] = A->realp[1*IA1][0*IA0];
h[N1/2][N0/2] = A->imagp[1*IA1][0*IA0];

// Unpack the two vectors from "vertical" storage:
for (j1 = 1; j1 realp[(2*j1+0)*IA1][0*IA0]
            + i * A->realp[(2*j1+1)*IA1][0*IA0]
    h[j1][N0/2] = A->imagp[(2*j1+0)*IA1][0*IA0]
            + i * A->imagp[(2*j1+1)*IA1][0*IA0]
}

// Take regular elements:
for (j1 = 0; j1 realp[j1*IA1 + j0*IA0]
             + i * A->imagp[j1*IA1 + j0*IA0];
    h[j1][N0-j0] = conj(h[j1][j0]);
}

// Perform Discrete Fourier Transform.
for (k1 = 0; k1 realp[k1*IC1 + k0*IC0] = Re(H[k1][2*k0+0]);
    C->imagp[k1*IC1 + k0*IC0] = Im(H[k1][2*k0+1]);
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fft2d_zrop

Computes a 2D forward or inverse out-of-place, single-precision real FFT.

vDSP_fft2d_zropD

Computes a 2D forward or inverse out-of-place, double-precision real FFT.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fft2d_zropt

Computes a 2D forward or inverse out-of-place, single-precision real FFT using a temporary buffer.

vDSP_fft2d_zroptD

Computes a 2D forward or inverse out-of-place, double-precision real FFT using a temporary buffer.

## See Also

### Functions for 2D Real FFT

In-Place Functions for 2D Real FFT

Perform fast Fourier transforms in place on 2D real data.

