<!-- tyhp-readme:start -->
# tyhpdef/symfony-console

Tyhp type definitions for `symfony/console` `8.1.7`.

```bash
composer require --dev tyhpdef/symfony-console:8.1.7
```

This is a metapackage. Composer also installs `tyhpdef/symfony-console-impl` (type files).
Require **this** name, not `tyhpdef/symfony-console-impl`.

See https://tyhplang.com.

## Maintain `symfony/console`? Ship the types yourself

If you are a Packagist maintainer of `symfony/console`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-console-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/console` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-console": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/console` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/console` with a real constraint,
   `"replace": { "tyhpdef/symfony-console": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/console` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-console` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
