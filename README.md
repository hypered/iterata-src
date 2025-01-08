# Lex Iterata - Source pages

[Lex Iterata](https://refli.be/fr/lex) is a project to collect and transform
the content of the Belgian Official Journal web site. It presents that content
in an enhanced format for human comprehension, while also providing structured
data tailored for machine consumption. This Git repository stores the original
content, as downloaded from the Belgian Official Journal web site, and
converted to UTF-8.

Normally, for any given file, something like the following commands should
return no differences:

```
$ curl -s https://www.ejustice.just.fgov.be/eli/ordonnance/2019/04/25/2019012116/justel | iconv -f windows-1252 -t utf-8 > a
$ git diff --no-index texts/2019/01/2019012116.html a
```

**Note**: In practice, differences can occur: we don't recreate the whole
collection of files when we update this repository (we add missing files from
time to time), but the documents on the Belgian Official Journal can change.

This repository contains 206115 legislative texts.

Last updated: 2025-01-08.
