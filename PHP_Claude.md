✅ PHP Project Rules (Strict OOP, DDD, Elegant Objects)

###CI & Workflow

All CI workflows must pass before code changes may be reviewed.

The existing code structure must not be changed without a strong reason.

Every bug must be reproduced by a unit test before being fixed.

Every new feature must be covered by a unit test before implementation.

Minor inconsistencies or typos in the existing code may be fixed.

README.md must be short, purposeful, and free from grammar mistakes or duplicated documentation.

###Code Style & Design

Every class must have a docblock describing its purpose and providing usage examples.

Every method and function must have a docblock.

Docblocks must be written in English using UTF-8.

Classes must follow DDD and Elegant Objects principles.

Classes must be final unless there is a strong architectural need.

Class names must not end with the “-er” suffix.

Each class must have exactly one primary constructor; secondary constructors must delegate to it.

Each class must encapsulate 1–4 attributes.

Utility classes are prohibited.

Static methods are prohibited.

Getters and setters must be avoided; encapsulation must be achieved through behavior.

Immutable objects must be favored.

Methods must respect CQRS: queries must be nouns, commands must be verbs.

Method names must be single verbs; variable names must be single nouns.

No blank lines inside method bodies.

No comments inside method bodies.

Paired Brackets principle must be respected.

Implementation inheritance is prohibited (subtyping via interfaces is allowed).

Methods must not return null; objects or exceptions must be used.

null may not be passed as an argument.

Type introspection and casting are prohibited.

Reflection on object internals is prohibited.

Public methods that do not come from an interface must be avoided.

Error and log messages must be a single sentence with no periods at the end.

Favor fail-fast: throw exceptions early with maximum context.

##Testing

Every change must be covered by a unit test.

Each test case may contain only one assertion, and it must be the last statement.

Each test file must map one-to-one with the feature it tests.

Test names must be full English sentences describing behavior.

Tests may not share state or use setUp()/tearDown() idioms.

Tests may not use static literals or shared constants.

Tests must close all used resources.

Tests must use irregular and non-ASCII inputs.

Tests must not assert on error messages or codes.

Tests must not rely on default configurations; they must provide all inputs explicitly.

Tests may not mock the filesystem, sockets, or memory managers; prefer fake objects and stubs.

Tests should create large fixtures at runtime and inline small fixtures.

Tests must use ephemeral TCP ports when required.

Tests must not print log messages or rely on log output.

Tests must not rely on Internet connectivity.

Tests must be robust against concurrency issues and verify concurrency when applicable.

Tests must retry potentially flaky blocks.

Tests must prepare a clean state instead of cleaning up afterward.

Test method names must write “cannot” and “dont” without apostrophes.
