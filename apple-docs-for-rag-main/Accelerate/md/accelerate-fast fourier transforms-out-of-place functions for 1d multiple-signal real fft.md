

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 1D Multiple-Signal Real FFT 

API Collection

# Out-of-Place Functions for 1D Multiple-Signal Real FFT

Perform fast Fourier transforms out of place on multiple-signal 1D real data.

## Overview

The functions in this group use the following operation for a forward real-to-complex transform:

```
N = 1 realp[m*IMA + j*IA];
         h[2*j + 1] = A->imagp[m*IMA + j*IA];
     }

     // Perform Discrete Fourier Transform.
     for (k = 0; k realp[m*IMC + 0*IC] = Re(H[ 0 ]).
     C->imagp[m*IMC + 0*IC] = Re(H[N/2]).

     // Store regular components:
     for (k = 1; k realp[m*IMC + k*IC] = Re(H[k]);
         C->imagp[m*IMC + k*IC] = Im(H[k]);
     }
}

```

The functions in this group use the following operation for an inverse complex-to-real transform:

```
N = 1 realp[m*IMA + 0*IA];
    h[N/2] = A->imagp[m*IMA + 0*IA];
    for (j = 1; j realp[m*IMA + j*IA]
           + i * A->imagp[m*IMA + j*IA];
        h[N-j] = conj(h[j]);
    }

    // Perform Discrete Fourier Transform.
    for (k = 0; k realp[m*IMC + k*IC] = H[2*k+0];
        C->imagp[m*IMC + k*IC] = H[2*k+1];
    }
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fftm_zrop

Computes a forward or inverse out-of-place, single-precision real FFT on multiple signals.

vDSP_fftm_zropD

Computes a forward or inverse out-of-place, double-precision real FFT on multiple signals.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fftm_zropt

Computes a forward or inverse out-of-place, single-precision real FFT on multiple signals using a temporary buffer.

vDSP_fftm_zroptD

Computes a forward or inverse out-of-place, double-precision real FFT on multiple signals using a temporary buffer.

## See Also

### Functions for 1D Multiple-Signal Real FFT

In-Place Functions for 1D Multiple-Signal Real FFT

Perform fast Fourier transforms in place on multiple-signal 1D real data.

