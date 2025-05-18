# gerium vcpkg registry

To add the repository, create the following `vcpkg-configuration.json` file next to your `vcpkg.json` file and add the following content to it:

```json
{
  "$schema": "https://raw.githubusercontent.com/microsoft/vcpkg-tool/main/docs/vcpkg-configuration.schema.json",
  "default-registry": {
    "kind": "git",
    "baseline": "b02e341c927f16d991edbd915d8ea43eac52096c",
    "repository": "https://github.com/microsoft/vcpkg"
  },
  "registries": [
    {
      "kind": "git",
      "repository": "https://github.com/VladimirShaleev/gerium-assets",
      "reference": "vcpkg-registry",
      "baseline": "f7293c18e566cf6dc044963498abf523e3b4c30e",
      "packages": [
        "fidelityfx",
        "fidelityfx-sc",
        "imgui",
        "joltphysics"
      ]
    }
  ]
}
```
