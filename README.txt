libffi-compat provides update-libffi-compat, a script which uses
pkg-config to find the libffi include directory and create symbolic
links to the headers in /usr/include (where they should go in the
first place).

Some software like cffi in lisp and python like to assume a fixed
location for software, so needing pkg-config is a problem.  Just run
update-libffi-compat as root to create links to solve this.

libffi-compat is in the public domain, use it for whatever.
