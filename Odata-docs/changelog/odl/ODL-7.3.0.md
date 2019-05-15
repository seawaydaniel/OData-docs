---
title: "ODataLib 7.3.0"
description: "ODataLib 7.3.0 release notes"

---

## Changes in ODataLib 7.3.0 Release ##

> [!NOTE]
> ODataLib 7.3.0 adds support key features including optional function parameters, parser support for the $compute clause, primitive type casts, and the ability to read and write untyped data as structured values. 

## Features ##

[[[#760](https://github.com/OData/odata.net/issues/760)] Aggregation not supported for dynamic properties

[[#782](https://github.com/OData/odata.net/issues/782)] Add support for optional parameters in function

[[#799](https://github.com/OData/odata.net/issues/799)] Support for $compute in $select and $filter

[[#800](https://github.com/OData/odata.net/issues/800)] Support for structured reading/writing of untyped values

[[#801](https://github.com/OData/odata.net/issues/801)] Supporting Primitive Type Casts

## Fixed Bugs ##

[[Issue #747](https://github.com/OData/odata.net/issues/747)] Cannot select dynamic property of a dynamic property 

[[Issue #814](https://github.com/OData/odata.net/issues/814)] Support writing enum-valued Annotations

[[Issue #856](https://github.com/OData/odata.net/issues/856)] Raw Value serializer output json string for Spatial type


This release delivers OData core libraries including ODataLib, EdmLib and Spatial. OData Client for .NET is not published in this release.