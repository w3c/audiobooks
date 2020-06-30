# Audiobooks Manifest Schema

The schema in [this directory](https://github.com/w3c/audiobooks/tree/master/schema) is an adaptation of the publication manifest schemas for validating audiobook manifests. (Note, however, that not all constraints can be captured through the schemas.)

The schema is written in [JSON Schema](https://json-schema.org/), and currently conform to **Draft-07**.

The schema is updated to newer drafts as broad support in validators becomes available. 

## Structure

The primary schema file `audiobooks.schema.json` also requires several [component schemas](https://github.com/w3c/audiobooks/tree/master/schema) from the publication manifest repository (currently all the json files except `publication.schema.json`). These schema files need to be downloaded and placed in the same directory.

Only the primary schema file needs to be specified for validation as the other files are automatically imported.

## Validators

A [list of JSON Schema validators](https://json-schema.org/implementations.html) and the draft(s) they support is available from the JSON Schema site.

The audiobooks manifest schema is known to work with the following validators/tools:

- [ajv-cli](https://github.com/jessedc/ajv-cli)
- [Oxygen Editor](https://www.oxygenxml.com/)
