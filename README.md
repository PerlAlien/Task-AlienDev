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

Other prereqs may be added in the future if they are deemed useful for [Alien](https://metacpan.org/pod/Alien) development.

# CAVEATS

This module does require Perl 5.22 or better currently because at least some of its prereqs
require that version.  Note that [Alien](https://metacpan.org/pod/Alien)s authored with these tools should work on Perls
of at least 5.8.4 or better, so this is just a _development_ requirement.

# AUTHOR

Graham Ollis <plicease@cpan.org>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2021 by Graham Ollis.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
