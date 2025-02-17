# Revision history for patch

## Unreleased

* Rewrite `PatchMapWithMove` in terms of `PatchMapWithPatchingMove`.
  Care is taken to make this not a breaking change.
  In particular, `PatchMapWithMove` is a newtype of `PatchMapWithPatchingMove`, as is the `NodeInfo` and `From` of `PatchMapWithPatchingMove`'s versions of those.
  There are complete constructor and field patterns too, and everything is
  exported under the newtype as real constructors and fields would be.

## 0.0.4.0

* Enable PolyKinds

## 0.0.3.2

* Update version bounds

## 0.0.3.1

* Replace `fromJust` with something easier to debug.

## 0.0.3.0

* Create `PatchMapWithPatchingMove` variant which supports moves with a patch.

* Create `DecidablyEmpty` subclass of `Monoid`.

## 0.0.2.0

* Consistently provide:

   - `Wrapped` instances

   - `*WithIndex` instances

   - `un*` newtype unwrappers

  for `PatchMap`, `PatchIntMap`, and `PatchMapWithMove`.

## 0.0.1.0

* Support older GHCs with `split-these` flag.

* Additional instances for the `Group` class for basic types.

## 0.0.0.1

* Remove unneeded dependencies

## 0.0.0.0

* Extract patching functionality from Reflex.
