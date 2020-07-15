# Ursus Atom

A library for manipulating Urbit atoms and auras.

## Usage

Ursus contains a submodule for working with [atoms and auras](https://urbit.org/docs/tutorials/hoon/atoms-auras-and-simple-cell-types/), with support for the urbit phonetic base:

```swift
let ship = try! PatP(string: "~lanrus-rinfep")
let point = Int(ship) // 328448
```

There is an `Aura` protocol with an associated type `Atom` which can be any `UnsignedInteger` type, but in practice we use `BigUInt` types.

Current implementations:

- `PatP` (`@p`)
- `PatQ` (`@q`)
- `PatUV` (`@uv`)

## Installation

Ursus Atom can be installed using Cocoapods by adding the following lines to your podfile:

```ruby
pod 'UrsusAtom', '~> 1.0'
```

I can probably help set up Carthage or Swift Package Manager support if you need it.

## Todo list

Things that would make this codebase nicer:

- [ ] Additional atom and aura types.
- [ ] Better documentation/examples.

## Other utilities

- [util.js](https://github.com/urbit/urbit/blob/master/pkg/interface/src/lib/util.js)
- [urbit-ob](https://github.com/urbit/urbit-ob)
- [urbit-hob](https://github.com/urbit/urbit-hob)

## Dependencies

- [BigInt](https://github.com/attaswift/BigInt)
- [MurmurHash-Swift](https://github.com/daisuke-t-jp/MurmurHash-Swift)
- [Parity](https://github.com/dclelland/Parity)
