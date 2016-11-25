# Simple YAML

There are some special chars in YAML, eg: `@ & *`. `&` is used for Anchors
but it almost won't used in validr's schema.
Those chars are conflict with validr's schema syntax, so I modified
YAML parser, treat `@ &` as plain text and disable Anchor syntax of YAML.

Also, this parser load YAML mapping as OrderedDict and use SafeLoader by default.


## Install

    pip install simple-yaml


## Usage

    import simple_yaml as yaml

## License

MIT License
