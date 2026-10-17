# Committed dataset

**Source dataset:** NYC TLC yellow taxi trips, January 2023

**Selection:** Systematic source-order sample: every 50th row, starting at row 0, from 3,066,766 source records. Original source fields retained; this is not the complete month.

**Data license:** [NYC Open Data terms / public TLC records](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page). This applies to the data, independently of the project code.

## Sources

- https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
- https://d37ci6vzurychx.cloudfront.net/trip-data/yellow_tripdata_2023-01.parquet

## CSV files

| File | Rows | Bytes |
|---|---:|---:|
| [yellow_taxi_2023_01_sample.csv](raw/yellow_taxi_2023_01_sample.csv) | 61,336 | 6,439,393 |

Attribution: NYC Taxi and Limousine Commission and reporting providers. Parquet converted to CSV without invented trips. Completed pickups are a sampled activity proxy, not full demand counts or observations of available supply/unserved demand. Account for sampling when aggregating; one month limits temporal generalization. Timestamp anomalies and other source-quality problems are retained for audit.

The CSV files contain published observations or their documented format conversion; no training records were invented. Source formats and raw CSV exports are distinguished by the manifest. File checksums and schemas are recorded in [csv-manifest.json](csv-manifest.json).
