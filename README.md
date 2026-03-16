# publicholidaydata

Public holiday datasets for client apps.

## Files

- `data/au_holidays.json`
  - Compatibility format used by ParkTimer now.
  - Keys: `version`, `country`, `country_code`, `states`.

- `data/public_holidays_v2.json`
  - Extensible multi-country format.
  - Includes `country_name`, per-region data, and multi-year grouping.

- `data/parking_rules_v1.json`
  - Parking sign rule catalog for ParkTimer runtime updates.

- `data/parking_rules_schema_v1.json`
  - JSON schema for validating `parking_rules_v1.json`.

## Update flow

1. Edit JSON files.
2. Bump `version` / `dataset_version`.
3. Commit and push.
4. Use GitHub Raw URL in your app settings.
