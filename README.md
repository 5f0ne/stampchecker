# Description

Check timestamp manipulation based on TSK body file. The result list all directories and files within the TSK body file, where the creation time comes after other timestamps. All timestamps uses UTC.

# Installation

`pip install stampchecker`

# Usage

**From command line:**

`python -m stampchecker add --path PATH`

| Option | Short | Type | Default | Description |
|---|---|---|---|---|
|--path | -p | String | - | Path to TSK body file |


# Example

`python -m stampchecker -p tsk-body.txt`

```
################################################################################

Stamp Checker by 5f0
Check timestamp manipulation based on TSK body file

Current working directory: path/to/stampchecker

Investigated file: ./tsk-body.txt

 Datetime: 01/01/1970 10:11:12

################################################################################

              ---> /dir/01.jpg
-------------------
    Creation Time: 2012-12-27 14:23:14+00:00 - 1356618194
-------------------
Modification Time: 2012-05-20 18:33:16+00:00 - 1337538796
     Changed Time: 2012-12-27 14:14:09+00:00 - 1356617649
-------------------

Execution Time: 0.000259 sec
```

# License

MIT