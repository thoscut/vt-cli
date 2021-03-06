## vt scan file

Scan one or more files

### Synopsis

Scan one or more files.

This command receives one or more file paths and uploads them to VirusTotal for
scanning. It returns the file paths followed by their corresponding analysis IDs.
You can use the "vt analysis" command for retrieving information about the
analyses.

If the command receives a single hypen (-) the file paths are read from the standard
input, one per line.

```
vt scan file [file]... [flags]
```

### Examples

```
  vt scan file foo.exe
  vt scan file foo.exe bar.exe
  cat list_of_file_paths | vt scan file -
```

### Options

```
  -h, --help          help for file
  -t, --threads int   number of threads working in parallel (default 5)
```

### Options inherited from parent commands

```
  -k, --apikey string   api key
  -v, --verbose         verbose output
```

### SEE ALSO

* [vt scan](vt_scan.md)	 - Scan files or URLs

###### Auto generated by spf13/cobra on 25-Jun-2020
