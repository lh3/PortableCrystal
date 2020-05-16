Crystal is a young compiled programming language that is similar to Ruby in
syntax but is much faster. It is non-trivial to install Crystal without the
root permision. Although you can find precompiled binary packages from Crystal's
[release page][rel], those packages lack essential libraries required to
compile any Crystal programs. As a result, users have to install additional
packages to make Crystal work.

This repository provides portable precompiled Crystal binaries. The only
difference from the official packages is that pacakges here include static
[libevent][libev] and [PCRE][pcre] libraries. Users can download a package,
unpack it and run `crystal-verion_x64-linux/bin/crystal` to compile their
programs without installing other libraries. Another benefit of using our
packages is that the compiled executable is not dynamically linked to the two
libraries and is thus more portable.

At present, this repository does not provide libyaml and libgmp which are
required to compile certain programs.

[rel]: https://github.com/crystal-lang/crystal/releases
[libev]: https://libevent.org/
[pcre]: https://www.pcre.org/
