
  Crowd Control Copy - cccp
=============================

Cccp is intended as a way to organize file transfers in batch computing systems.
When you have multiple machines that need to copy files from a central server at
the same time, they might overload the server and lead to bad performance. Using
cccp you avoid these problems.

Cccp checks for lock files in the source directory and delays any copy action
until the number of lock files is below a certain threshold. While copying, it
creates a new lockfile in the directory.
