# Contribution to Arctium Projects

You can contribute to Arctium projects with issues and PRs. Simply filing issues for problems you encounter is a great way to contribute. Contributing implementations is greatly appreciated.

## Reporting Issues

We always welcome bug reports, API proposals and overall feedback. Here are a few tips on how you can make reporting your issue as effective as possible.

## Contribution

### Contributor License Agreement

You must sign a Arctium Contribution License Agreement (CLA) before your PR will be merged. This is a one-time requirement for projects at Arctium. You can read more about [Contribution License Agreements (CLA)](http://en.wikipedia.org/wiki/Contributor_License_Agreement) on Wikipedia.

The agreement: [arctium-contribution-license-agreement.pdf](arctium-contribution-license-agreement.pdf)

You don't have to do this up-front. You can simply clone, fork, and submit your pull-request as usual. When your pull-request is created, it is classified by a CLA bot. If the change is trivial (for example, you just fixed a typo), then the PR is labelled with `cla-not-required`. Otherwise it's classified as `cla-required`. Once you signed a CLA, the current and all future pull-requests will be labelled as `cla-signed`.

### Line Endings

- Please be sure to make use of **"Unix-like"** line endings `\n`.
- Every file should end with an empty newline.

Our provided [EditorConfig](.editorconfig) file should help with that.

### File Headers

The following file header is used for all Arctium projects. Please use it for new files.

```
// Copyright © Arctium.
// Licensed under the MIT License (MIT). See License.md file in the repository root for more information.
```

### Global Usings

We make use of some global usings to define our own types or to prevent excessive usings in file headers.
Please make sure to include those in every project root in a file named `GlobalUsings.cs`

```
// Copyright © Arctium.
// Licensed under the MIT License (MIT). See License.md file in the repository root for more information.

global using int8 = sbyte;
global using int16 = short;
global using int32 = int;
global using int64 = long;
global using int128 = System.Int128;

global using uint8 = byte;
global using uint16 = ushort;
global using uint32 = uint;
global using uint64 = ulong;
global using uint128 = System.UInt128;

global using float16 = System.Half;
```

### Type Usages

When using internal runtime types be sure to use those defined in the `GlobalUsings.cs` file.

