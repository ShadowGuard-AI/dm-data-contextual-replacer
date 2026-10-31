![Banner](banner.png)

# dm-data-contextual-replacer
Replaces data based on contextual keywords identified nearby. For instance, if 'salary' or 'income' appears within N words of a number, replace the number with a masked value. Requires a pre-defined list of contextual keywords. - Focused on Tools designed to generate or mask sensitive data with realistic-looking but meaningless values

## Install
`git clone https://github.com/ShadowGuardAI/dm-data-contextual-replacer`

## Usage
`./dm-data-contextual-replacer [params]`

A number with punctuation attached, such as `50000,` beside a keyword, is masked and the punctuation is kept in the output. When no value is replaced, the run prints `No values were replaced.` and exits 1.

## Parameters
- `-h`: Show help message and exit
- `--input`: The input text to process.
- `--keywords`: Comma-separated list of contextual keywords.
- `--window_size`: The number of words to check around the target (default: 10).
- `--replacement_value`: The value to replace matched data with. If not provided, a random float is generated.
- `--faker_locale`: The Faker locale to use for generating replacement values (default: en_US).
- `--log_level`: Set the logging level (default: INFO).

## License
Copyright (c) ShadowGuardAI
