
  Crowd Control Copy - cccp
=============================

Cccp is intended as a way to organize file transfers in batch computing
systems. When you have multiple machines that need to copy files from a
central server at the same time, they might overload the server and lead to bad
performance. Using cccp you avoid these problems.

Cccp checks for lock files in a `.cccp` directory inside the source directory
and delays any copy action until the number of lock files is below a certain
threshold. While copying, it creates a new lockfile.

  USAGE
---------

    cccp [arguments] <source> <destination>

  Arguments
-------------

    -A <lock-dir>
        Create the lock files in <lock-dir> instead of at the source.
    -D  Create the lock files at the destination instead of the source.
    -h  Show the help text and exit.
