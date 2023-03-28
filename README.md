LevelDB is a fast key-value storage library written at Google that provides an ordered mapping from string keys to string values.

[![ci](https://github.com/google/leveldb/actions/workflows/build.yml/badge.svg)](https://github.com/google/leveldb/actions/workflows/build.yml)

# Notes

**we write learning nodes in Notes/ dir and write comments in source code files.**

# Features

* Multiple changes can be made in one atomic batch.
* Users can create a transient snapshot to get a consistent view of data.
* Data is automatically compressed using the [Snappy compression library](https://google.github.io/snappy/).

# Documentation

  [LevelDB library documentation](https://github.com/google/leveldb/blob/main/doc/index.md) is online and bundled with the source code.

# Building

Getting source

```bash
git clone --recurse-submodules git@github.com:infdahai/leveldb-note.git
```

Quick start:

```bash
mkdir -p build && cd build
cmake -DCMAKE_BUILD_TYPE=Release .. && cmake --build . -j$(nproc)
```

clang-format:

```bash
clang-format -i --style=file <file>
```

## Repository contents

See [doc/index.md](doc/index.md) for more explanation. See
[doc/impl.md](doc/impl.md) for a brief overview of the implementation.
