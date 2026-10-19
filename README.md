# L&C Revit AI Assistant: releases

This repository holds only built update packages and the update manifest for the L&C Revit AI Assistant add-in. There is no source code here.

- `manifest.json` lists the available packages. The add-in's loader reads it from
  `https://raw.githubusercontent.com/Jackieson888/lc-revit-assistant-releases/main/manifest.json`.
- Each package is a zip attached to a GitHub Release (`vX.Y.Z`). The manifest gives its download URL and SHA-256 hash; the loader rejects any download whose hash doesn't match.

Packages are published with `installer/publish-release.ps1` in the source repository. Don't edit `manifest.json` by hand unless you're removing a bad version.
