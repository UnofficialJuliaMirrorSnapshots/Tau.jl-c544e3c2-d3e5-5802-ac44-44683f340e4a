# Tau.jl

<div align="center"><img src="https://rawgit.com/JuliaMath/Tau.jl/master/tau-2pi.svg" width="300"/></div><br/><br/>

[![travis][travis-img]](https://travis-ci.org/JuliaMath/Tau.jl)
[![appveyor][appveyor-img]](https://ci.appveyor.com/project/waldyrious/tau-jl)
[![codecov][codecov-img]](http://codecov.io/github/JuliaMath/Tau.jl)

[travis-img]: https://img.shields.io/travis/JuliaMath/Tau.jl/master.svg?label=Linux,%20macOS
[appveyor-img]: https://img.shields.io/appveyor/ci/waldyrious/tau-jl/master.svg?label=Windows
[codecov-img]: https://img.shields.io/codecov/c/github/JuliaMath/Tau.jl/master.svg?label=coverage

This [Julia](https://github.com/JuliaLang/julia) [package](http://pkg.julialang.org/)
defines the [Tau](http://www.tauday.com/tau-manifesto) constant
and related functions.

```
tau ≈ 2*pi
```

## Usage

After installing this package with `Pkg.add("Tau")`, it can be used as follows:

```julia
using Tau

tau == τ ≈ 2*pi  # => true
typeof(tau)      # => Irrational{:τ}
```

Note: to input the τ character, type `\tau` then press <kbd>Tab</kbd>.

The tau variants of `sinpi`, `cospi`, and `mod2pi` are also defined:

```julia
sintau(1//4) # => 1.0
costau(1//2) # => -1.0
```

## The tau != 2pi inequality

When this package was first created, the equality `tau == 2pi` did hold true,
in accordance to the mathematical definition of the constant.
However, that is not valid anymore -- the two values are only approximately equal: `tau ≈ 2*pi`.

For a detailed explanation of the reasons for this, see [this document](tau-2pi-equality.md).
