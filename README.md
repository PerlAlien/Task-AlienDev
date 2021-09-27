# Task::AlienDev ![static](https://github.com/PerlAlien/Task-AlienDev/workflows/static/badge.svg) ![linux](https://github.com/PerlAlien/Task-AlienDev/workflows/linux/badge.svg)

Task bundle for Alien development

# SYNOPSIS

```
$ cpanm Task::AlienDev
```

# DESCRIPTION

This [Task](https://metacpan.org/pod/Task) bundle is useful for those doing [Alien](https://metacpan.org/pod/Alien) development.  Installing it will give
you these modules:

- [Alien::Build](https://metacpan.org/pod/Alien::Build)

    Framework for writing [Alien](https://metacpan.org/pod/Alien)s.

- [Alien::MSYS](https://metacpan.org/pod/Alien::MSYS)

    Is used on Windows to make autoconf style packages work.

- [App::af](https://metacpan.org/pod/App::af)

    The `af` command line application for working with [alienfile](https://metacpan.org/pod/alienfile)s.

- [Dist::Zilla::MintingProfile::AlienBuild](https://metacpan.org/pod/Dist::Zilla::MintingProfile::AlienBuild)

    The [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) minting profile for creating [Alien::Build](https://metacpan.org/pod/Alien::Build) based [Alien](https://metacpan.org/pod/Alien)s.

- [Dist::Zilla::Plugin::AlienBuild](https://metacpan.org/pod/Dist::Zilla::Plugin::AlienBuild)

    Some useful [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla) plugins useful for developing [Alien::Build](https://metacpan.org/pod/Alien::Build) based [Alien](https://metacpan.org/pod/Alien)s.

The latest versions as of when this [Task](https://metacpan.org/pod/Task) was released should be installed at minimum if
they are not already installed.

In addition these modules, which are dynamic dependencies on some platforms, are installed:

- [Env::ShellWords](https://metacpan.org/pod/Env::ShellWords)
- [File::Listing](https://metacpan.org/pod/File::Listing)
- [HTTP::Tiny](https://metacpan.org/pod/HTTP::Tiny)
- [Mojo::DOM58](https://metacpan.org/pod/Mojo::DOM58)
- [Sort::Versions](https://metacpan.org/pod/Sort::Versions)
- [URI](https://metacpan.org/pod/URI)

Having these dynamic dependencies pre-installed makes it easier to test [Alien](https://metacpan.org/pod/Alien)s in both
`share` and `system` modes.

Other prereqs may be added in the future if they are deemed useful for [Alien](https://metacpan.org/pod/Alien) development.

# CAVEATS

This module does require Perl 5.22 or better currently because at least some of its prereqs
require that version.  Note that [Alien](https://metacpan.org/pod/Alien)s authored with these tools should work on Perls
of at least 5.8.4 or better, so this is just a _development_ requirement.

This [Task](https://metacpan.org/pod/Task) indirectly requires both [Alien::FFI](https://metacpan.org/pod/Alien::FFI) and [Alien::Libarchive3](https://metacpan.org/pod/Alien::Libarchive3).  If you do
not want to build them from source or do not have internet access where the build is
happening you will want to pre-install `libffi` and `libarchive`.  On Debian based systems
you can do that with `sudo apt-get update && sudo apt-get install libffi-dev libarchive-dev`.

# AUTHOR

Graham Ollis <plicease@cpan.org>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2021 by Graham Ollis.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
