# Hello World

- run `yarn format:md` (`prettier --write README.md`)
- expected: README.md is reformatted
- actual: parsing error

## Investigation

The parser option in .prettierrc.js is always used, even when the parser extensions do not match the file type. This could be considered a reasonable default... but maybe there could be a warning?
