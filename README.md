# Tillage Extension Specification

- **Title:** Tillage
- **Identifier:** <https://fiboa.github.io/tillage-extension/v0.2.0/schema.yaml>
- **Property Name Prefix:** tillage
- **Extension Maturity Classification:** Proposal
- **Owner**: TBD

This document explains the Tillage Extension to the
[Field Boundaries for Agriculture (fiboa) Specification](https://github.com/fiboa/specification).

This extension describes whether tillage has been performed on a field, along with various attributes
to describe the tillage.

- Examples:
  - [GeoJSON](examples/geojson/)
  - [GeoParquet](examples/geoparquet/)
- [Schema](schema/schema.yaml)
- [Changelog](./CHANGELOG.md)

## Properties

The fields in the table below can be used in these parts of fiboa documents:

- [ ] Collection
- [x] Feature Properties

| Property Name    | Type    | Description |
| ---------------- | ------- | ----------- |
| tillage:occurred | boolean | **REQUIRED.** Whether or not this field has had a tillage event in a calendar year. |
| tillage:type     | string  | The type of tillage that occurred. |
| tillage:events   | int32   | Number of tillage passes in a calendar year. |
| tillage:depth    | double  | Depth of soil disturbance in centimeters. |
| tillage:spacing  | double  | Space in centimeters between disks. |
| tillage:angle    | float   | Degrees of the disk of the tillage equipment. (0 - 90). |

**tillage:type** allowed values:

- `conventional`
- `conservation`
- `unknown`

## Contributing

See the [contributing guideline](CONTRIBUTING.md) for more details.
