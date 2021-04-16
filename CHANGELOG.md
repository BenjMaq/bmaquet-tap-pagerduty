# Changelog

## 1.0.1
  * Replace `start_date` by `since`, as `start_date` does not exists in the PagerDuty API https://developer.pagerduty.com/api-reference/reference/REST/openapiv3.json/paths/~1incidents/get , but `since` exists. 
  * Add `excluded_fields[]` to `valid_params` of class `IncidentsStream()`. This new `excluded_fields[]` is used to exclude `log_entries` and `alerts` fields if they are not needed.
  * Add `replication_method` to `valid_params` of class `IncidentsStream()`. This allows to pass `INCREMENTAL` replication method for the `incidents` stream.
 
## 1.0.0
  * This is a fork of https://github.com/singer-io/tap-pagerduty v0.2.0.