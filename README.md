# Introduction to mdBook tool

Generating a simple documentation webpage using mdBook tool.

## References

- mdBook tools
	1. [mdBook - Official repository](https://github.com/rust-lang/mdBook).
	1. [mdBook - Introduction](https://rust-lang.github.io/mdBook/index.html).
	1. [MdBook variables preprocessor](https://crates.io/crates/mdbook-variables).

- mdBook themes
	1. [Catppuccin for mdBook](https://github.com/catppuccin/mdBook).
	1. [mdBook - Theme](https://github.com/zjp-CN/mdbook-theme).

- mdBook related articles
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

- Features
	1. [x] Generate the documentation pages from Markdown `.md` files.
	1. [x] Write documents with variables support.
	1. [x] Custom Catpuccin themes (Frappé, Latte, Macchiato, Mocha).
	1. [x] Generate and host a web site on **GitHub Pages**.
	1. [x] Embedded required binaries for Linux.

## Setup

### Installation

There is no need to install mdBook tool on your operating system once all required binaries files to generate the documentation was embedded into this project and they were compiled to run in any Linux distribution (including WSL2).

- In example of Visual Studio Code be sure to run the `deploy script` from WSL terminal.

<p align="center" width="100%">
    <img width="33%" src="../assets/images/script_deploy.png">
    <img width="33%" src="./docs/assets/images/script_deploy.png">
</p>

<!--
![Deploy script](./docs/assets/images/script_deploy.png).
-->

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

- For an easy management, use the `deploy` script. Type `./deploy --help` to display the help message.

### Publishing

Once the following requirements are attempted, then the generated contents are going to be available at [Example mdBook hosted on GitHub Pages](https://henrikbeck95.github.io/example_mdbook/dist/).

- Requirements
    1. [x] Documentation is built.
    1. [x] Repository is commited and pushed to branch `main`.