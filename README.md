# Midll Configuration Language

Midll is a modern, human-friendly configuration language designed for clarity, structure, and explicit typing. It supports both brace-based and indentation-based sections, type annotations, references, and arrays, making it ideal for application, infrastructure, and data configuration.

## Features
- **Explicit type annotations**: Every assignment specifies its type (`string`, `int`, `bool`).
- **Sections and nesting**: Use either braces `{}` or indentation for nested sections.
- **Arrays of records**: Group related values in arrays.
- **References/interpolation**: Use `${path.to.value}` to reference other values.
- **Comments**: Use `#` for comments.
- **Readable and strict**: Designed for both humans and machines.

## Example
```midll
project: {
    name: string = "Production Example"
    authors: string = [
        name: Jade Larafey
        email: jade@midll.com
    ]
}

server:
    host: string = "0.0.0.0"
    port: int = 443
    enable_tls: bool = true

base_uri: string = "https://midll.com"
docs_uri: string = "${base_uri}/docs"
```

## Grammar
Midll is formally specified in both ABNF and EBNF grammars:
- `midll.abnf`
- `midll.ebnf`

## Usage
- Use Midll for configuration files where clarity, type safety, and references are important.
- Parsers can be generated or implemented using the provided ABNF/EBNF grammars.

## Project Structure
- `midll.abnf`, `midll.ebnf`: Language grammars
- `example.midll`: Example configuration file
- `CHANGELOG.md`: Project history
- `docs/`: Documentation

## License
See `LICENSE` for details.

---
For more information, see the grammar files and example config, or open an issue in this repository.
