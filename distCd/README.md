# distCd

Flat JSON dataset of administrative records. Each object represents one administrative entry.

---

## Fields

| Key               | Type   | Nullable | Description                                          |
| ----------------- | ------ | -------- | ---------------------------------------------------- |
| `distCd`          | string | No       | Code value of the record                             |
| `levCd`           | number | No       | Level code                                           |
| `provName`        | string | No       | Province name                                        |
| `provAbbr`        | string | Yes      | Province abbreviation                                |
| `provAbbrName`    | string | Yes      | Province short name                                  |
| `provDistCd`      | string | Yes      | Province-level code reference                        |
| `cityName`        | string | Yes      | City name                                            |
| `cityAbbr`        | string | Yes      | City abbreviation                                    |
| `cityAbbrName`    | string | Yes      | City short name                                      |
| `cityDistCd`      | string | Yes      | City-level code reference                            |
| `ctyName`         | string | Yes      | County/District name                                 |
| `ctyAbbr`         | string | Yes      | County abbreviation                                  |
| `ctyAbbrName`     | string | Yes      | County short name                                    |
| `source`          | string | No       | Source label (e.g. `provinces`, `citys`, `countrys`) |
| `statCd`          | string | No       | Status code                                          |
| `createdTime`     | number | Yes      | Created timestamp                                    |
| `createdTimeStr`  | string | Yes      | Created time (string)                                |
| `modifiedTime`    | number | Yes      | Modified timestamp                                   |
| `modifiedTimeStr` | string | Yes      | Modified time (string)                               |

---

## Notes

* The dataset is flat (no nesting).
* Some fields may be `null` depending on the record.
* Multiple rows may represent the same place with different `source` values.
