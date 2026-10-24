# Overseer demo

A deliberately flawed Next.js + Supabase source sample for [Overseer](https://github.com/gipotenuzsa/overseer).
It was generated with AI for analyzer demonstrations. All credential-shaped values
are synthetic. Do not deploy it or connect it to a real database.

## Try it

Run with the published Overseer package:

```sh
git clone https://github.com/gipotenuzsa/overseer-demo.git
cd overseer-demo
npx overseer-cli
```

You can also install the Overseer release tarball and run `overseer`, or
use `pnpm cli ui <path-to-this-folder>` from the Overseer source repository.
The sample itself does not need npm install or a running web server.

Open Results to follow its files and data. Review a critical finding and copy its
fix prompt. Compare the intentionally flawed commit with the clean baseline:

```sh
overseer diff --since clean-baseline
overseer check
```

The default scan has 4 critical, 4 warning, and 2 informational findings, with health
18. The diff also reports the new nanoid dependency. `check` intentionally exits 1.
[EXPECTED.md](EXPECTED.md) describes each trigger, including an optional synthetic
environment-file exercise. Never use real credentials. The baseline and current
sample are analysis fixtures, not production-ready application templates.

MIT licensed. See the main repository for docs, releases, and contribution details.
