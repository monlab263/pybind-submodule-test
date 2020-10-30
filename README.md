this repo is test for `pybind` installation as submodule.

docs: https://pybind11.readthedocs.io/en/stable/installing.html


## Include as a submodule

When you are working on a project in Git, you can use the pybind11 repository as a submodule. From your git repository, use:

```
git submodule add ../../pybind/pybind11 extern/pybind11 -b stable
git submodule update --init
```

This assumes you are placing your dependencies in `extern/`, and that you are using GitHub; if you are not using GitHub, use the full https or ssh URL instead of the relative URL `../../pybind/pybind11` above. Some other servers also require the `.git` extension (GitHub does not).

From here, you can now include `extern/pybind11/include`, or you can use the various integration tools (see [Build systems](https://pybind11.readthedocs.io/en/stable/compiling.html#compiling)) pybind11 provides directly from the local folder.

