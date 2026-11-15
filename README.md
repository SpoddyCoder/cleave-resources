# cleave-resources

Mirrored models, presets, and other resources [Cleave](https://github.com/SpoddyCoder/cleave) downloads at runtime.

Cleave downloads these files on first use. Each one is pinned by SHA-256, so Cleave accepts a copy from this mirror or from the upstream source only if it matches the hash exactly. This mirror is tried first; the upstream source stays as a fallback.

The files are not part of this git tree. Each one is attached to a GitHub Release, tagged by resource and version.

## Resources

| Resource | Release tag | File | Upstream | License |
| --- | --- | --- | --- | --- |
| Beat This `final0` checkpoint | `beat-this-final0-v1` | `beat_this-final0.ckpt` | [CPJKU/beat_this](https://github.com/CPJKU/beat_this) | MIT, see [beat-this/LICENSE](beat-this/LICENSE) |

Details and hashes for each resource are in its folder.

## Licensing

Nothing here is licensed as a whole. Each resource keeps its upstream license and copyright notice, in a `LICENSE` file in its folder and in its release notes. The authors of these resources are not affiliated with Cleave and do not endorse it.

Only resources whose license allows redistribution are mirrored here.

## Adding a resource

1. Create a folder named for the resource. Add the upstream `LICENSE`, copied exactly, and a `README.md` with the upstream link, file size, and SHA-256.
2. Create a release tagged `<resource>-v<n>`, attach the file unmodified, and put the license notice and SHA-256 in the release notes. Do not mark it as the latest release.
3. Add a row to the table above.

Never replace a published file. Cleave pins each file's hash, so a changed file needs a new tag (`-v2`), and the old release stays up for older Cleave builds.
