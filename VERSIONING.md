# Versioning

Our packages follow [Semantic Versioning](https://semver.org). Given a version `MAJOR.MINOR.PATCH`,
we bump the:

- `MAJOR` version for a breaking change,
- `MINOR` version for a backwards compatible addition,
- `PATCH` version for a backwards compatible fix.

Versions below `1.0.0` are still stabilizing, and a `MINOR` bump may break you.

This policy covers the public API of a package. Anything documented as internal or private may change
in any release.

## Backwards compatible

- Adding a function, type, module, or package.
- Adding an optional parameter that has a default.
- Adding a field to a payload or struct that we construct and you read.
- Widening the set of inputs an existing function accepts.
- Deprecating something without removing it.
- Changing internals, performance, logging, or documentation.

## Breaking

- Removing or renaming anything public, including a field.
- Adding a required parameter.
- Narrowing the set of inputs an existing function accepts, including adding a validation rule to an
  input that previously allowed it.
- Changing the type of a public parameter, field, or return value.
- Changing the meaning of an existing value while keeping its name and type.
- Raising the minimum supported language, runtime, or platform version.
- Removing support for a platform we previously supported.

## Cases where ecosystems disagree

When an ecosystem is ambiguous, we take the stricter reading and treat the change as breaking.

- Adding a variant to a public enum or a member to a public interface, since exhaustive matching and
  implementing types make this observable to you.
- Adding a callback to a behaviour or a required method to a protocol or trait.
- Changing an exception, error type, or error value that you may be matching on.

## Deprecation

We deprecate before we remove. A deprecated API keeps working for at least one `MINOR` release, and
the deprecation notice says what to use instead. Removal happens in the next `MAJOR` release.

## Security

A fix for a security vulnerability may break backwards compatibility when there is no safe
alternative. See our [Security Policy](./SECURITY.md).
