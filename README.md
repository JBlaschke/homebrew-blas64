# Homebrew-BLAS64

`openblas64`: A formula for a 64-bit version of OpenBLAS. In order to avoid
conflicts with existing installations of BLAS (which might rely on the 32-bit
interface), we add the `64_` sufftix. This formula was built using:
`make SYMBOLSUFFIX=64_ INTERFACE64=1 BINARY=64 ...`

This tap also includes formulae that use this 64-bit version of openBLAS:
1. `julia64`: A version of Julia built with `USE_BLAS64=1`. **Note**: this
formula conflicts with the "regular" `julia` cask/formula (as they link to the
same julia executable).

## Installation

```
brew tap JBlaschke/homebrew-blas64
```

## References

1. The `objconv` formula is based on:
https://github.com/hawkw/homebrew-grub/blob/master/Formula/objconv.rb