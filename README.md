# manageiq-nuage-docs
Repository for generating documentation for the Nuage Networks provider for ManageIQ

## Compile into PDF
First edit [main.adoc](./nuage_provider_configuration/main.adoc) and uncomment appropriate
variable set (either ManageIQ or CloudForms).

Then install [`asciidoctor-pdf`](https://asciidoctor.org/docs/asciidoctor-pdf) gem and use it like
this to compile .adoc documentation into a PDF file: 

```bash
bundle exec asciidoctor-pdf nuage_provider_configuration/main.adoc -o ./PREVIEW.pdf
```

Command above will create file `./PREVIEW.pdf` that can be used as documentation preview.

