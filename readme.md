
# MP3Cat

MP3Cat is a fast command-line utility for merging MP3 files without re-encoding.

    $ mp3cat --help

    Usage: mp3cat [FLAGS] [OPTIONS] [ARGUMENTS]

      This tool concatenates MP3 files without re-encoding. It can join constant
      bit-rate (CBR) files, variable bit-rate (VBR) files, or a mixture of both.

      If a set of input CBR files share the same bit-rate, the output file will
      also be CBR; if the input files have different bit-rates, the output file
      will be VBR.

      Files to be merged can be specified as a list of filenames:

        $ mp3cat one.mp3 two.mp3 three.mp3

      Alternatively, an entire directory of .mp3 files can be merged:

        $ mp3cat --dir /path/to/directory

    Arguments:
      [files]                 List of files to merge.

    Options:
      -d, --dir <path>        Directory of files to merge.
      -i, --interlace <path>  Interlace a spacer file between each input file.
      -o, --out <path>        Output filename. Defaults to 'output.mp3'.

    Flags:
      -f, --force             Overwrite an existing output file.
      -h, --help              Display this help text and exit.
      -q, --quiet             Run in quiet mode.
      -t, --tag               Copy the ID3 tag from the first input file.
      -v, --version           Display the application's version number and exit.

See the project's [homepage][] for details and binary downloads.

[homepage]: https://darrenmulholland.com/dev/mp3cat.html
