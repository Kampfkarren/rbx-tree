# rbx_reflection Changelog

## Unreleased Changes

## 3.1.384 (2019-05-12)
* Changed getters on descriptor objects to be now marked `#[inline]`
* Added `RbxClassDescriptor::is_service`

## 3.0.384 (2019-05-12)
* Updated reflection database to client 0.384.1.302070
* Added inference for `Content` values from string literals
* Breaking: rewrote reflection database to have a much more conservative public API
* Breaking: introduced the concept of canonical properties and serialization-only properties, which makes handling serialized files much easier.
* Breaking: changed the `ValueResolveError` type to be a struct, which makes it more opaque and less prone to breakage.
* Breaking: renamed version constants to have an `RBX_` prefix.

## 2.0.377 (2019-03-20)
* Updated reflection database to client 0.377.1.289039

## 2.0.374 (2019-03-01)
* Updated to `rbx_dom_weak` 1.0
* Updated reflection database
* Removed default values for some properties like `Parent`
* Added `tags` field (of type `RbxInstanceTags`) to `RbxInstanceClass`

## 1.0.373 (2019-02-26)
* Adjusted version number scheme again to account for patches to the library
* Added `ValueResolveError` to public interface

## 0.2.373 (2019-02-25)
* Adjusted version number to include client release number
* Added default values for serialized properties
* Added version constants
* Added type resolution function, `try_resolve_value`

## 0.1.0 (2019-02-14)
* Initial release
* Exposes a reflection database for instances and enums
* Supports resolving ambiguous `rbx_dom_weak` values