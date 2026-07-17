# What does this implement/fix?

<!-- Quick description and explanation of changes -->

## Types of changes

<!-- Release notes are generated from PR labels, so apply the matching label as well. -->

- [ ] Bugfix (non-breaking change which fixes an issue) — label: `bugfix`
- [ ] New device (adds a configuration for a new device) — label: `new-device`
- [ ] Enhancement (non-breaking change which improves an existing configuration) — label: `enhancement`
- [ ] Breaking change (fix or change that alters existing behaviour, e.g. renamed entities or changed pins) — label: `breaking-change`
- [ ] Dependency update (actions, reusable workflows or ESPHome version) — label: `dependencies`
- [ ] Other

**Related issue (if applicable):**

- fixes <link to issue>

## Checklist

- [ ] The configuration compiles and has been tested on the actual device.
- [ ] `yamllint --strict .` passes.

If a device configuration was added or renamed:

- [ ] The device directory contains both `<device>.yaml` (core config) and `<device>.factory.yaml` (factory wrapper).
- [ ] `dashboard_import.package_import_url` points to the core YAML in this repository.
- [ ] `update.source` points to the correct `https://firmware.esphome.io/<directory>/<device>/manifest.json` URL.
- [ ] The factory YAML is named `<device>.factory.yaml` so CI picks it up automatically.
- [ ] The device is listed in the dropdown in `.github/ISSUE_TEMPLATE/bug_report.yml`.
- [ ] The README is updated if it lists supported devices.
