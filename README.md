# Software Factory

Software Factory is a Codex-based system for turning a declared product vision and a selected roadmap milestone into a runnable candidate with evidence. It builds toward each product's declared goals while leaving decisions about those goals with the product's governing party. Within the authorized build scope, the factory chooses implementation details.

The [factory product specification](product.json) describes the intended factory. The [build contract](build-contract.json) defines the exchange with a product repository, and its [request schema](build-request.schema.json) validates the shape of a request. A product repository supplies its own specification, roadmap, acceptance scenarios and a small build request. Music Composer is the first consumer.

## Factory accounting

The factory tracks resources consumed by specification work, build runs and verification. The [ledger template](costs/ledger.template.json) distinguishes measured usage, charges, estimates and unknowns. Actual cost records belong in a private accounting store and are not published with this reusable factory specification. Product operating costs remain with each product.

## Shared ontology

This repository pins the [product ontology](dependencies/product-ontology/ontology.json) as a Git submodule. The factory is itself a product governed and assessed using that shared vocabulary. This repository contains a declaration and interface, not a working build service yet.

## License

This project is available under the [MIT License](LICENSE).
