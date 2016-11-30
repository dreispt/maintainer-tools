

OCA addon modules can be categorized according to their maturity, as:

  * Beta
  * Stable
  * Mature

**Beta** modules can be merged and available on OCA branches,
but still need improvements before they are categorized as Stable.
They are not guaranteed to be API-stable nor maintained, 
and even risk being later removed. 
Because of this they are not suitable for deployment in production,
and feature a visible warning banner at the top of the README description.
They must also keep an open GitHub Issue, with the to-do list for the module,
and the link to it in the README.
Their version number should be 0.Y.Z.

**Stable** modules are production quality, 
and future changes are expected to be API-stable.
Their version number should be >= 1.0.0.

When a Beta module is promoted to Stable, the major version number should
be increased to 1, and the banner is removed from the README.

**Mature** modules meet all Stable criteria,
plus a few extra criteria to make them more robust and easier to use.
For example, to have this label they are required to have 
good quality documentation and a high code test coverage ratio.
This is signalled in the README though a banner with a star.

To be promoted from Stable to Mature we need a PR that improves it
so that it meets all the criteria, and adds the star banner to the README.


The point for Mature modules is to give incentive and recognize the extra
work to make modules more robust and easier to use.
These are things like an excellent code test coverage,
a detailed and useful README and documentation,
or being available though a Configuration option.

The point for Beta modules is to allow faster PR merges.
Instead of a PR being repeatedly improved by the author until all the
reviewers are happy with it, we instead assume this first PR as the
starting point for a stable module. This improvement work can split
into subsequent PRs, until it can be considered stable.
These are smaller, easier to review, and faster to merge.
And instead of a series of "no" until you get a "yes", 
you have a more motivating series of "ok" until you get a "yes".

A GitHub Issue should be used to coordinate the efforts of the 
ongoing PRs, and to keep track of the list of changes that need
to be implemented (or are just nice to have).

Beta modules require at least one contributor to be committed to
work on the work plan. Beta modules that do net meet this criteria 
can be removed from the OCA branch. A pointer for the revision of
last version of the module will be kept in the Issue, 
so that it is always possible for someone else to recover and
continue the work.
