# trove-parliament-press-releases-refugees

*A GLAM Workbench data repository*

Trove includes more than 380,000 press releases, speeches, and interview transcripts issued by Australian federal politicians and saved by the Parliamentary Library. This dataset contains metadata and full text of items from the press releases collection that include the term 'refugees' (or a number of related terms).

The dataset was created in two stages. First, Trove was searched for relevant resources, and metadata from each search result was saved in a CSV file. Then links to ParlInfo contained within the metadata were used to download the full text.

Known issues:
- some items had no downloadable text available in Parlinfo, so the number of text files is less than the number of metadata records
- some items have different metadata but the same text, for example when a press release is issued by both a political party and an individual member
- because of the way Trove groups records, it's possible some of the records don't include any of the search terms.

These datasets were generated using notebooks in the [trove-government](https://github.com/GLAM-Workbench/trove-government/) repository.

For more information and documentation see the [Trove government](https://glam-workbench.net/trove-government) section of the [GLAM Workbench](https://glam-workbench.net).

## Dataset summary
- [text](https://github.com/GLAM-Workbench/trove-parliament-press-releases-refugees/tree/main/text/) (directory containing 14,145 files)
- [results.csv](https://github.com/GLAM-Workbench/trove-parliament-press-releases-refugees/blob/main/results.csv) (12.9 MB, text/csv)


## Dataset details

### [text](https://github.com/GLAM-Workbench/trove-parliament-press-releases-refugees/tree/main/text/)

|                 |                                                                                                                                                                                                                                                                  |
|:----------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| date harvested  | 2024-02-15                                                                                                                                                                                                                                                       |
| number of files | 14,145                                                                                                                                                                                                                                                           |
| format          | directory                                                                                                                                                                                                                                                        |
| created by      | <a href='https://github.com/GLAM-Workbench/trove-government/blob/master/harvest-parliament-press-releases.ipynb'>Harvest parliament press releases from Trove</a>                                                                                                |
| query           | `nuc:"APAR:PR" AND ("illegal arrival" OR text:"immigrant" OR text:"immigrants" OR "asylum seeker" OR "boat people" OR refugee OR "boat arrivals")`                                                                                                               |
| description     | Contains individual text files, each containing the contents of an item from the press releases collection. Files are named using the following metadata fields: `date`, `contributor`, and `version_id`. For example: `1960-01-22-casey-richard-213589278.txt`. |
| license         | [Copyright Not Evaluated](http://rightsstatements.org/vocab/CNE/1.0/)                                                                                                                                                                                            |



### [results.csv](https://github.com/GLAM-Workbench/trove-parliament-press-releases-refugees/blob/main/results.csv)

|                |                                                                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| date harvested | 2024-02-20                                                                                                                                                        |
| file size      | 12.9 MB                                                                                                                                                           |
| format         | text/csv                                                                                                                                                          |
| created by     | <a href='https://github.com/GLAM-Workbench/trove-government/blob/master/harvest-parliament-press-releases.ipynb'>Harvest parliament press releases from Trove</a> |
| number of rows | 14225                                                                                                                                                             |
| query          | `nuc:"APAR:PR" AND ("illegal arrival" OR text:"immigrant" OR text:"immigrants" OR "asylum seeker" OR "boat people" OR refugee OR "boat arrivals")`                |
| license        | [CC0 Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)                                                                                |

#### Columns

| name           | type    | description                                                                                        |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------|
| `title`        | string  | nan                                                                                                |
| `contributor`  | string  | names of people and organisations contributing to this item; multiple values separated by | symbol |
| `date`         | date    | date when this item was presented or published; ISO format 'YYYY-MM-DD'                            |
| `description`  | string  | usually includes the beginning of the full text content (truncated at approx 200 characters)       |
| `type`         | string  | type of resource, eg 'Press Release' or 'Speech'; multiple values separated by | symbol            |
| `format`       | string  | format of resource, usually either 'Online Text' or empty; multiple values separated by | symbol   |
| `work_type`    | string  | Trove work format, eg 'Article'; multiple values separated by | symbol                             |
| `language`     | string  | language of resource, eg 'eng'; multiple values separated by | symbol                              |
| `extent`       | string  | often includes the number of pages; multiple values separated by | symbol                          |
| `rights`       | string  | information about copyright; multiple values separated by | symbol                                 |
| `subject`      | string  | subject or topic headings; multiple values separated by | symbol                                   |
| `is_part_of`   | string  | collection containing this item; multiple values separated by | symbol                             |
| `fulltext_url` | string  | Link to the full text version in ParlInfo                                                          |
| `trove_url`    | string  | link to the version record in Trove                                                                |
| `work_id`      | integer | Trove work identifier                                                                              |
| `version_id`   | integer | Trove version identifier                                                                           |
| `hash`         | string  | SHA-1 hash value generated from the full text; useful for identifying duplicate texts              |

----
Created by [Tim Sherratt](https://timsherratt.au) for the [GLAM Workbench](https://glam-workbench.net)