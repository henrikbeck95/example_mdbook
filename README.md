# mdBook - Example

Generating a simple documentation webpage using mdBook tool.

## References

1. [mdBook - Introduction](https://rust-lang.github.io/mdBook/index.html).
1. [mdBook - Theme](https://github.com/zjp-CN/mdbook-theme).
1. [mdBook: Uma Ferramenta Para Criar Documentações Utilizando Markdown](https://johnfercher.medium.com/mdbook-uma-ferramenta-para-criar-documenta%C3%A7%C3%B5es-utilizando-markdown-c30c9dfa5c9f).
1. [How I made a DOCUMENTATION WEBSITE for my Game Engine](https://www.youtube.com/watch?v=tJDof3nrfHU).

## Documentation

Generate a documentation webpage based on Markdown files.

- File structure
    1. All Markdown files **must be** at `./src/` directory folder path.
    1. Format your `./src/SUMMARY.md` file according to your needs.
    1. Configure your book using the `./book.toml` file.
    1. Customize your theme.
    1. The generated content files are stored at `./dist/` directory folder path.

## Setup

### Development

- Generate documentation
    > $ `mdbook build`

- The watch command can take a directory as an argument to use as the book's root instead of the current working directory.
    > $ `mdbook watch ./`

- Start the server up
    > $ `mdbook serve ./ -p 8000 -n 127.0.0.1`

- Open directly on browser
    > $ `xdg-open http://localhost:8000`

- The clean command is used to delete the generated book and any other build artifacts.
    > $ `mdbook clean`

### Publishing

Once the following requirements are attempted, then the generated contents are going to be available at [Example mdBook hosted on GitHub Pages](https://henrikbeck95.github.io/example_mdbook/dist/).

- Requirements
    1. [x] Documentation is built.
    1. [x] Repository is commited and pushed to branch `main`.
