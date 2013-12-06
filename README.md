# puppet-graphite

Puppet module for setting up Graphite, because it's no walk in the park manually. Built with
[Boxen](https://github.com/boxen/boxen) in mind.

## Usage

```puppet
include graphite
```

This will add carbon, whisper, and graphite-web.  If you prefer, each is configured as a puppet class.

## Required Puppet Modules

* `boxen`
* `homebrew`
* `nginx`
* `apache` ([mattheath/puppet-apache](https://github.com/mattheath/puppet-apache))
* `python` (depends on `xquartz`)
* `cairo` ([mattheath/puppet-cairo](https://github.com/mattheath/puppet-cairo), depends on `xz`, `pixman`, `libpng`, `pkgconfig`)

## Development

Write code. Run `script/cibuild` to test it. Check the `script` directory for
other useful tools.
