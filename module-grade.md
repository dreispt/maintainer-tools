

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

