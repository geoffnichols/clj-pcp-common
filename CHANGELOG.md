## 1.3.0

This is a maintenance release.

* update clj-parent to 3.1.1
* remove implementation of uuid?  If an alternative is needed, use kitchensink.core/uuid?

## 1.2.0

This is a feature release.

* Add support for Java 9.

## 1.1.4

This is a maintenance release

* Bumps clj-parent to 0.6.1, with i18n 0.8.0.

## 1.1.3

This is a maintenance release

* [PCP-731](https://tickets.puppetlabs.com/browse/PCP-731) Bump clj-parent to
  0.4.3 for i18n 0.7.1.

## 1.1.2

This is a maintenance release.

* [PCP-731](https://tickets.puppetlabs.com/browse/PCP-731) Bump i18n to 0.7.0
  to pickup a change in pot file name.
* Bump clj-parent to 0.4.1.

## 1.1.1

This is a maintenance release.

* Add a schema for the PCP v2 ErrorMessage, which did not previously match the
  specification.

## 1.1.0

This is a feature release.

* [PCP-600](https://tickets.puppetlabs.com/browse/PCP-600) Add schema
  definitions to be used in inventory updates. Additionally changes the
  return value of `uri-wildcard?` to be the exploded Uri in case it is a
  wildcard, or nil otherwise; this should not impact truthiness of the value.
* Bump clj-parent to 0.3.2

## 1.0.0

This is a major feature release introducing PCP v2. It continues to support PCP
v1, but breaks API compatibility for those using this library.

* [PCP-645](https://tickets.puppetlabs.com/browse/PCP-645) Add PCP v2 protocol

## 0.5.5

This is a maintenance release

* [PCP-620](https://tickets.puppetlabs.com/browse/PCP-620) Validate chunk
  lengths when decoding to prevent DOS

## 0.5.4

This is a maintenance release

* Updates clj-i18n to 0.4.3 for a bug introduced in 0.4.2

## 0.5.3

This is a maintenance release

* Updates clj-i18n to 0.4.2 for a performance-related bug fix

## 0.5.2

This is a maintenance release

* [PCP-525](https://tickets.puppetlabs.com/browse/PCP-525) Explicitly
  validate the Message argument of the message/encode function.
* [PCP-535](https://tickets.puppetlabs.com/browse/PCP-535) Don't run tests
  with schema validation enabled.
* [PR #26](https://github.com/puppetlabs/clj-pcp-common/pull/26) Update
  dependencies to be consistent with upstream projects.

## 0.5.1

This is a maintenance release

* [PCP-367](https://tickets.puppetlabs.com/browse/PCP-367) Add i18n library
  and mark text strings for extraction.
* [PCP-467](https://tickets.puppetlabs.com/browse/PCP-467) Disable Prismatic
  Schema validation by default.
* [PCP-483](https://tickets.puppetlabs.com/browse/PCP-483) Fix InventoryRequest
  schema. It was overly broad in relation to the definition at
  pcp-specifications.

## 0.5.0

This is a feature release.

This is the first public release to clojars.

* [PCP-42](https://tickets.puppetlabs.com/browse/PCP-42) Added schema for
  `http://puppetlabs.com/version_error` message bodies.
* [PCP-45](https://tickets.puppetlabs.com/browse/PCP-45) Release to clojars
  rather than internal nexus servers.

## 0.4.1

This is a maintenance release

* [CTH-311](https://tickets.puppetlabs.com/browse/CTH-311) Updated
  Uri scheme from `cth` to `pcp`

## 0.4.0

* Renamed from former codenames to new component names.

## 0.2.0

* Removed server state from Message (CTH-328)
* Removed add-hops function
* Added add-debug add-json-debug functions
* Now verify that MessageId looks like a uuid

## 0.1.0

* Added prismatic schema schema.core/defn decorations to the rest of
  the public api functions (CTH-206)
* Renamed Endpoint -> Uri, and reworked envelope schema for changes to
  cthun specifications (CTH-210)

## 0.0.1

* Initial internal release, extracted from cthun server (CTH-185)
* Added set-expiry
* Added Message schema and made make-message constrain to it.
