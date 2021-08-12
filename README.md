# PineAPPL grids for NNPDF
In this repository grids generated from the
[runcards](https://github.com/NNPDF/runcards) repository are stored.

## Usage
To use the grids first install PineAPPL's CLI, see it's [README] for
instructions. You then have a command-line program `pineappl` that you can use
to perform convolutions, calculate PDF uncertainties, write plotting scripts,
etc.:

    pineappl convolute ATLAS_DY_7TEV_49FB_HIMASS.pineappl.lz4 NNPDF31_nlo_as_0118_luxqed
    pineappl pdf_uncertainty ATLAS_DY_7TEV_49FB_HIMASS.pineappl.lz4 NNPDF31_nlo_as_0118_luxqed
    pineappl --silence-lhapdf plot ATLAS_DY_7TEV_49FB_HIMASS.pineappl.lz4 NNPDF31_nlo_as_0118_luxqed > plot.py && python plot.py

There are more subcommands available. Consult

    pineappl --help

to get an overview of all subcommands, and

    pineappl convolute --help

to get a summary of all options for a specific subcommand.

[README]: https://github.com/N3PDF/pineappl#readme
