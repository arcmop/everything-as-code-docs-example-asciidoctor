# Everything as Code - Documentation - Asccidoc y Asciidoctor example

## Detail
- **asciidoc**: AsciiDoc is a plain text markup language for writing technical content. It’s packed with semantic elements and equipped with features to modularize and reuse content. AsciiDoc content can be composed using a text editor, managed in a version control system, and published to multiple output formats
  
- **asciidoctor**: Asciidoctor is a fast, open source, text processor for parsing AsciiDoc into a document model and converting it to output formats such as HTML 5, DocBook 5, man(ual) pages, PDF, and EPUB 3. Asciidoctor is written in the Ruby programming language.

## How to build a PDF file:

```sh

#Build inside of container

$ docker run --rm -it -v $PWD:/documents/ asciidoctor/docker-asciidoctor:1.18
bash-5.1$ asciidoctor-pdf document.adoc -D dist
bash-5.1$ exit

#Oneline command
$ docker run --rm -it -v $PWD:/documents/ asciidoctor/docker-asciidoctor:1.18 asciidoctor-pdf document.adoc -D dist
```

## Links
- https://docs.asciidoctor.org/
- https://asciidoc.org/