Best Practices for Projects in the Blosc Ecosystem
==================================================

Contributing and Git
--------------------

* ``master`` should always be stable and it should be possible to release from
  it at any time.
* Only minor things and release preperation should be done on ``master``.
* Development and bugfixing should happen in feature branches.
* All feature branches should be submitted as pull-requests from the users.
  forks. This means: no feature branches in the main repository.
* All branches must include tests if at all possible and ideally also an entry
  in the changelog.

Relasing
--------

* The release procedure should be documented.
* All tags should alwyas be signed with a gpg-key.

Continuous Integration
----------------------

* At least a basic Travis CI config should be used
* For Python projects, test against all supported versions of Python.
