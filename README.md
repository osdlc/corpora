# models

This repository is a holding pen. It is where the shared models will live once they have
matured: the profiles, the packs and the starter corpora that the sdlc product and other tools
build on.

For now the work happens in [osdlc/osdlc](https://github.com/osdlc/osdlc). The models are
developed there, beside `corpus-schema` and the sdlc product that uses them, so that a change that
crosses them is one pull request. A model package moves here when it nears 1.0 and releases on its
own. [osdlc/osdlc#789](https://github.com/osdlc/osdlc/pull/789) records the decision and the plan.

Please open issues and pull requests in osdlc/osdlc, not here.

## What is here

- [`system-cleanup/profile`](system-cleanup/profile/) (`@osdlc/corpus-profile-system-cleanup`): record types for a
  cited record of where tools and apps keep data that can be reclaimed from disk, built on the
  claims profile.
- [`system-cleanup/reference`](system-cleanup/reference/): that record. 68 stores (package
  managers, toolchain managers, build tools and SDKs, OS package managers, model runtimes and
  hubs, container runtimes and editors), each asked six questions, every answer backed by quotes
  checked against their pages. host-cleaner's plugins are built from it.

Check them with `pnpm install` and `pnpm run validate` at the root.
