# pythoneda-sandbox/python

A Python project used to test PythonEDA.

## How to declare it in your flake

Check the latest tag of the artifact repository: https://github.com/pythoneda-sandbox/python-artifact/tags, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-shared-sandbox-python = {
      [optional follows]
      url =
        "github:pythoneda-sandbox/python-artifact/[version]?dir=python";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [https://nixos/nixpkgs](nixpkgs "nixpkgs") and [https://github.com/numtide/flake-utils](flake-utils "flake-utils").

The Nix flake is under the [https://github.com/pythoneda-sandbox/python-artifact/tree/main/python](python "python") folder of <https://github.com/pythoneda-sandbox/python-artifact>.

