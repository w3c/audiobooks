# Audiobooks Manifest Schema

The schema in [this directory](https://github.com/w3c/audiobooks/tree/master/schema) is an adaptation of the publication manifest schemas for validating audiobook manifests. (Note, however, that not all constraints can be captured through the schemas.)

The schema is written in [JSON Schema](https://json-schema.org/), and currently conform to **Draft-07**.

The schema is updated to newer drafts as broad support in validators becomes available. 

## Structure

The primary schema file `audiobooks.schema.json` requires the shared [component schemas](https://github.com/w3c/pub-manifest/tree/master/schema/) from the publication manifest repository. The `module` folder from that repository may need to be downloaded and placed in the same directory as the `audiobooks.schema.json` file depending on the validator used.

In some cases, it may be possible to validate without downloading the physical schemas (i.e., if the validator can retrieve the schemas automatically). In these cases, only the URL `https://w3c.github.io/audiobook/schema/audiobooks.schema.json` needs to be specified.

## Validators

A [list of JSON Schema validators](https://json-schema.org/implementations.html) and the draft(s) they support is available from the JSON Schema site.

The audiobooks manifest schema is known to work with the following validators/tools:

- [ajv-cli](https://github.com/jessedc/ajv-cli)
- [Oxygen Editor](https://www.oxygenxml.com/)
