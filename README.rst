Best Practices for Projects in the Blosc Ecosystem
==================================================

Contributing and Git
--------------------

* ``master`` should always be stable and it should be possible to release from
  it at any time.
* Only really trivial things should be done on ``master``.
* Development and bugfixing should happen in feature branches.
* All feature branches should be submitted as pull-requests from the user's
  forks. This means: no feature branches in the main repository.
* All branches must include tests if at all possible and ideally also an entry
  in the changelog.
* Any pull-request should be based on the current position of ``master`` before
  merging by using rebase. This is not such a strict requirement because the
  pull-requests and resulting merges are more important, but it is definitely
  an advantage.

Releasing
---------

* The release procedure should be documented.
* All tags should always be signed with a gpg key.

Continuous Integration
----------------------

* At least a basic Travis CI config should be used.
* For Python projects, test against all supported versions of Python.

Shipping c-blosc Sources
------------------------

If c-blosc sources are to be included, please store the sources in ``c-blosc``
sources subdirectory. And use the ``subtree-merge-blosc.sh`` script to include
new versions.

General Policies
----------------

* The role of the maintainer is to enforce process
* Pull-requests, issues and mailinglist posts, should be responded to as soon
  as possible

Licences
--------

All licenses should be kept in a directory ``LICENSES``. In case c-blosc sources
are included in the project's Git repository inherited licenses should be
symlinked into the ``LICENSES`` directory to avoid duplication.
