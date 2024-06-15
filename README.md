[![Written in TypeScript](https://flat.badgen.net/badge/icon/TypeScript?icon=typescript&label)](http://www.typescriptlang.org/) [![npm](https://flat.badgen.net/npm/v/@mtti/uuid?icon=npm&label)](https://www.npmjs.com/package/@mtti/uuid) [![License](https://flat.badgen.net/github/license/mtti/uuid-ts)](https://github.com/mtti/uuid-ts/blob/master/LICENSE)

Branded UUID types for Typescript.

Partially wraps the [uuid](https://www.npmjs.com/package/uuid) package to produce branded strings for supported UUID versions, validated with regular expressions. Causes no runtime changes to the strings.

Supports version 4 UUIDs.

## Types

### UUID

Any supported UUID version. This is a normal Javascript `string` type branded with a unique symbol indicating the UUID version it represents.

### UUIDvX

Same as `UUID` but for a specific UUID version.

## Functions

### uuid4

Generate a version 4 UUID.

### isUUID

Type guard for the type `UUID`.

Check if a value of unknown type is a valid string representation of any supported UUID version.

### isUUIDvX

Same as `isUUID` but for a specific UUID version.

### asUUID

Return a value of unknown type as an `UUID` if it is a valid string representation of any supported UUID type, otherwise return `null`.

### asUUIDvX

(Replace X with number of any supported UUID version)

Same as `asUUID` but for a specific UUID version.

### expectUUID

Same as `asUUID` but throws an error if the value is not a valid UUID.

### expectUUIDvX

(Replace X with number of any supported UUID version)

Same as `expectUUID` but for a specific UUID version.
