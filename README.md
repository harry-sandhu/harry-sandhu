# Harry Sandhu

I write backend systems and the full-stack products built on top of them, with a
weak spot for projects where the constraint is the interesting part: a permission
model that has to hold up under tests, a 1.44MB disk image, a crypto scheme where
the server is deliberately not allowed to know anything.

## Projects

**[Campfire](https://github.com/harry-sandhu/Campfire)** - an internal ticketing
system, the kind of thing most teams either skip building or bolt together with a
single admin flag. I built the permission model first: groups, roles, and an audit
log that gets checked by integration and end-to-end tests, not just assumed to
work. Express and MongoDB on the backend, Next.js on the front. [Live demo](https://www.autodao.tech)

**[ROTOR](https://github.com/harry-sandhu/ROTOR)** - a drone-building tool where
the hard problem is compatibility, not the UI. Instead of a wall of warning text
telling you a part won't fit, the rules live in a typed API, so an invalid
configuration can't reach the screen in the first place. Bun and Turborepo
monorepo, Fastify and Drizzle against Postgres, one contracts package shared end
to end.

**[FloppyRogue](https://github.com/harry-sandhu/FLOPPYROUGE)** - a roguelite built
for a contest with a genuinely absurd rule: the whole game has to fit on a 1.44MB
floppy disk, 1,474,560 bytes, no exceptions. No engine, no external libraries, a
software-rendered framebuffer, procedurally generated levels, and an audio engine
synthesized in code because shipping real sound files would blow the budget.
Current build uses about 90% of that budget, assets included.

**[Web3-encrypted-files-vault](https://github.com/harry-sandhu/Web3-encrypted-files-vault)**
- a file vault built so the server never sees a plaintext file or a key.
Encryption happens client-side with AES-GCM, and the key is derived from a wallet
signature plus a PIN, so only the wallet owner can ever decrypt what gets
uploaded.

**[website-auditor](https://github.com/harry-sandhu/website-crawler)** - a CLI
that drives an actual browser instead of just parsing HTML, then runs SEO,
accessibility, performance, and security checks against what it finds. The
security side stays scoped to the target host and rate-limited by default, with
an explicit flag required before anything more active runs.

**Cinder** - private startup work, so there isn't much I can show. It's a
semantic runtime that turns tagged UI into something a voice or text command can
act on, resolving locally against a graph of the app before it ever reaches out
to a model. [usecinder.dev](https://www.usecinder.dev/)

## Currently

Splitting time between Cinder and a handful of backend and systems side
projects, most of which end up here eventually. Still reach for C or C++ when a
project genuinely calls for it.

## Elsewhere

- Portfolio: [harry-sandhu.github.io/portfolio](https://harry-sandhu.github.io/portfolio/)
- LinkedIn: [harcharan-singh-5789b625a](https://www.linkedin.com/in/harcharan-singh-5789b625a)
- Email: singh.harcharan2003@gmail.com
