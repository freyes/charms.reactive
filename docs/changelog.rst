**Changelog**

0.6.3
^^^^^
Tuesday Apr 24 2018

* Export endpoint_from_name as well (#174)
* Rename Endpoint.joined to Endpoint.is_joined (#168)
* Only pass one copy of self to Endpoint method handlers (#172)
* Make Endpoint.from_flag return None for unset flags (#173)
* Fix hard-coded version in docs config (#167)
* Fix documentation of unit_name and application_name on RelatedUnit (#165)
* Fix setdefault on Endpoint data collections (#163)

0.6.2
^^^^^
Friday Feb 23 2018

* Hotfix for issue #161 (#162)
* Add diagram showing endpoint workflow and all_departed_units example to docs (#157)
* Fix doc builds on RTD (#156)

0.6.1
^^^^^

* Separate departed units from joined in Endpoint (#153)
* Add deprecated placeholder for RelationBase.from_state (#148)

0.6.0
^^^^^

* Endpoint base for easier interface layers (#123)
* Public API is now only documented via the top level charms.reactive namespace.
  The internal organization of the library is not part of the public API.
* Added layer-basic docs (#144)
* Fix test error from juju-wait snap (#143)
* More doc fixes (#140)
* Update help output in charms.reactive.sh (#136)
* Multiple docs fixes (#134)
* Fix import in triggers.rst (#133)
* Update README (#132)
* Fixed test, order doesn't matter (#131)
* Added FAQ section to docs (#129)
* Deprecations:

  * relation_from_name (renamed to endpoint_from_name)
  * relation_from_flag (renamed to endpoint_from_flag)
  * RelationBase.from_state (use endpoint_from_flag instead)

0.5.0
^^^^^

* Add flag triggers (#121)
* Add integration test to Travis to build and deploy a reactive charm (#120)
* Only execute matching hooks in restricted context. (#119)
* Rename "state" to "flag" and deprecate "state" name (#112)
* Allow pluggable alternatives to RelationBase (#111)
* Deprecations:

  * State
  * StateList
  * set_state (renamed to set_flag)
  * remove_state (renamed to clear_flag)
  * toggle_state (renamed to toggle_flag)
  * is_state (renamed to is_flag_set)
  * all_states (renamed to all_flags)
  * any_states (renamed to any_flags)
  * get_states (renamed to get_flags)
  * get_state
  * only_once
  * relation_from_state (renamed to relation_from_flag)

0.4.7
^^^^^

* Move docs to ReadTheDocs because PythonHosted is deprecated
* Fix cold loading of relation instances (#106)

0.4.6
^^^^^

* Correct use of templating.render (fixes #93)
* Add comments to bash reactive wrappers
* Use the standard import mechanism with module discovery
