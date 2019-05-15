---
title: "ODataLib 7.1.0"
description: "ODataLib 7.1.0 release notes"

---

## Changes in ODataLib 7.1.0 Release ##

### Migration to .NET Standard 1.1 ###

[[Commit a2af8c6c19f104f46b442df7f57f624ed77d82fc](https://github.com/OData/odata.net/commit/a2af8c6c19f104f46b442df7f57f624ed77d82fc)] Update profile111 to .netstandard1.1.

[[Commit 6f746cd0cd9d62a5bc57e345a910a6f9d8d4dc1b](https://github.com/OData/odata.net/commit/6f746cd0cd9d62a5bc57e345a910a6f9d8d4dc1b)] Adding new projects and solution for .NET Standard version of ODL.

Creating a new solution file for .NET Standard projects. Adding .NET
Standard versions of Microsoft.Spatial, Microsoft.OData.Edm,
Microsoft.OData.Core, and Microsoft.OData.Client. MSBuild doesn't
pre-process the dependency graph provided by the csproj files, so
explicitly spoonfeeding the chain in the Microsoft.Test.OData.DotNetStandard.sln
file.

Update build script to default to VS 2015 for .NET Standard,
removing NuGetPackage test project and deprecating
it, adding E2E .NET Standard project

Remove duplicate file: IEdmReferentialConstraint.cs.

Change version to 7.1.0

Note: "nuget restore" needs to be run manually on the new project
files for them to compile.

### New Features ###

[[Commit c0c6006a5a8683507c38623144a145de128851c6](https://github.com/OData/odata.net/commit/c0c6006a5a8683507c38623144a145de128851c6)] Adding support and tests for virtual property count.

[[Commit d064a1c6358130c581bb9d5bb32e774f8e921992](https://github.com/OData/odata.net/commit/d064a1c6358130c581bb9d5bb32e774f8e921992)] Adding support and tests for custom aggregation methods.

[[Commit 8e965e9f89951dbfea510e67cbbe89e4f75fa69b](https://github.com/OData/odata.net/commit/8e965e9f89951dbfea510e67cbbe89e4f75fa69b)] Add support for operations with no bindings.

## Fixed Bugs ##

[[Issue #525](https://github.com/OData/odata.net/issues/525)] Support for AnnotationPath.

[[Issue #526](https://github.com/OData/odata.net/issues/526)] Support for IncludeInServiceDocument.

[[Issue #680](https://github.com/OData/odata.net/issues/680)] Text "Date" will be parsed as "EDM.Date" type segment in URL parser.

[[Issue #687](https://github.com/OData/odata.net/issues/687)] Null exception when HttpHeaderValueElement.Value is not set.

[[Issue #706](https://github.com/OData/odata.net/issues/706)] Serialization exception when 2 subtypes define a property with the same name but different types.

[[Issue #758](https://github.com/OData/odata.net/issues/758)] countdistinct and $count are returning Edm.Int64 which is not spec compliant.

[[Issue #776](https://github.com/OData/odata.net/issues/776)] Fix ContextUrl generation for operations in path.

[[Issue #777](https://github.com/OData/odata.net/issues/777)] Fix trailing whitespace on empty line.

[[Issue #778](https://github.com/OData/odata.net/issues/778)] Fix tests and code for reading nested results from operations.

## Improvements ##

[[Commit 6e2dee52b37e620926cd0535f40d5537ba839c05](https://github.com/OData/odata.net/commit/6e2dee52b37e620926cd0535f40d5537ba839c05)] Add Test solutions for WP WindowsStore Portable.

[[Commit d695d6ded6d44fa3fdb7abbd5f8dc19c29330e10](https://github.com/OData/odata.net/commit/d695d6ded6d44fa3fdb7abbd5f8dc19c29330e10)] Update license.

[[Commit 8521d38405351f789134d8945a696a18eec929d3](https://github.com/OData/odata.net/commit/8521d38405351f789134d8945a696a18eec929d3)] Fix Phone Project.

[[Commit dc9632b686e47dba8a0bbeffb5cc8c5850e27c8b](https://github.com/OData/odata.net/commit/dc9632b686e47dba8a0bbeffb5cc8c5850e27c8b)] Fix fxcop issue.

[[Commit 3ea2d70d14c97344f43383d867a9edd81eb407a3](https://github.com/OData/odata.net/commit/3ea2d70d14c97344f43383d867a9edd81eb407a3)] Add test cases for DotNetCore.

[[Commit 2ef3fc921ad4b557ef67cd17ce95eb08b33fa14e](https://github.com/OData/odata.net/commit/2ef3fc921ad4b557ef67cd17ce95eb08b33fa14e)] Update nuget.exe to 3.5.0 to resolve build issue with xunit.

[[Commit 0dc70678f05201ebc48c83219f6b4450078d0693](https://github.com/OData/odata.net/commit/0dc70678f05201ebc48c83219f6b4450078d0693)] Reordering comments to avoid compiler warnings.

[[Commit bbd9ede1e73de3538af6f1a223bcc7fe689688f4](https://github.com/OData/odata.net/commit/bbd9ede1e73de3538af6f1a223bcc7fe689688f4)] Update test project to copy the new and old version of the EntityFramework.nuspec file.

[[Commit 6eb8a4b5ecff1d83d883a95162d187ee3a44f935](https://github.com/OData/odata.net/commit/6eb8a4b5ecff1d83d883a95162d187ee3a44f935)] Remove use of StringBuilder.Clear() for .NET 3.5 support.

[[Commit c1edd714bf58ddd2876e10d31f0bd9ad81e25664](https://github.com/OData/odata.net/commit/c1edd714bf58ddd2876e10d31f0bd9ad81e25664)] Added metadata to tests for new bound function.

> [!NOTE]
> This release delivers OData core libraries including ODataLib, EdmLib and Spatial. OData Client for .NET is not published in this release.