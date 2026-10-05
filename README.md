<!-- tyhp-readme:start -->
# tyhpdef/nunomaduro-termwind

Tyhp type definitions for `nunomaduro/termwind` `2.4.0`.

```bash
composer require --dev tyhpdef/nunomaduro-termwind:2.4.0
```

This is a metapackage. Composer also installs `tyhpdef/nunomaduro-termwind-impl` (type files).
Require **this** name, not `tyhpdef/nunomaduro-termwind-impl`.

See https://tyhplang.com.

## Maintain `nunomaduro/termwind`? Ship the types yourself

If you are a Packagist maintainer of `nunomaduro/termwind`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/nunomaduro-termwind-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `nunomaduro/termwind` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/nunomaduro-termwind": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `nunomaduro/termwind` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `nunomaduro/termwind` with a real constraint,
   `"replace": { "tyhpdef/nunomaduro-termwind": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `nunomaduro/termwind` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/nunomaduro-termwind` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
