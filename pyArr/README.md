# pyArr

Flat JSON dataset mapping names to romanization fields.

---

## Fields

| Key     | Type   | Nullable | Description                           |
| ------- | ------ | -------- | ------------------------------------- |
| `code`  | string | No       | Code value of the entry               |
| `cName` | string | No       | Name in Chinese                       |
| `py`    | string | No       | Pinyin with spaces                    |
| `qp`    | string | No       | Full pinyin without spaces            |
| `jp`    | string | No       | Short pinyin (lowercase abbreviation) |

---

## Notes

* Each object represents a single name-to-romanization mapping.
* The dataset is flat (no hierarchy).
* Romanization fields are provided in multiple formats for different use cases.
