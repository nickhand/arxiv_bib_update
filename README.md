# arXiv bibtex updater
tool to search for and update out-of-date arXiv preprints in bibtex files

# installation
To install, simply run

```bash
pip install arxiv_bib_updater
```

# usage
The command-line options are available via:

```bash
arxiv_bib_updater -h
```

Given a bibtex file `out-dated-refs.bib` to search through, we can create a new file with updated references via:

```bash
arxiv_bib_updater out-dated-refs.bib -o fresh.bib
```

Note that you must create and specify your NASA ADS API token in order to query the ADS database. See https://github.com/adsabs/adsabs-dev-api#access for further details on creating this token. The token can be passed via the ``-h`` option on the command-line, or
stored in the file `~/.ads/dev_key` for repeated use. 
