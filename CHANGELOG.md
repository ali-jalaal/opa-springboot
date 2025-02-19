# OPA Spring Boot SDK Changelog

## v0.0.9 (unreleased)


## v0.0.8

* Change `build.gradle` to omit the `plain` classifier from the jar file it builds. This should make the default
  snippet show on https://central.sonatype.com/artifact/com.styra.opa/springboot _work as is_. Before, you would
  have to add `<classifier>plain</classifier>`.

## v0.0.7

* Bump `opa-java` version to 1.8.0.

## v0.0.6

* Fixed a null pointer exception while constructing the input to OPA with some Authentication implementations.

## v0.0.5

* Add `OPAAuthorizationManager` constructor that accepts a path and a `ContextDataProvider`, but not an `OPAClient`.
* `opa-java` is now marked as an `api` dependency in `build.gradle`, so it will not be transitively exposed to users.
* Bump `opa-java` version to 1.5.0.

## v0.0.4

* Explicitly mark the `ContextDataProvider` interface as public.
* Remove several unused dependencies, update remaining dependencies to latest stable versions.

## v0.0.3

* Add `OPAAuthorizationManager` constructor that accepts a path but not an `OPAClient`.

## v0.0.2

* Rather than hard-coding `en`, the preferred key to search for decision reasons for can now be changed with `OPAAuthorizationManager.setReasonKey()`. The default remains `en`.
* Update `build.gradle` to accurately reflect Apache 2 license.

## v0.0.1

* Initial release of the OPA Spring Boot SDK
