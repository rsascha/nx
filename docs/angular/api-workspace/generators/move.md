# move

Move an application or library to another folder

## Usage

```bash
nx generate move ...
```

```bash
nx g mv ... # same
```

By default, Nx will search for `move` in the default collection provisioned in `angular.json`.

You can specify the collection explicitly as follows:

```bash
nx g @nrwl/workspace:move ...
```

Show what will be generated without writing to disk:

```bash
nx g move ... --dry-run
```

### Examples

Move libs/my-feature-lib to libs/shared/my-feature-lib:

```bash
nx g @nrwl/workspace:move --project my-feature-lib shared/my-feature-lib
```

## Options

### destination

Type: `string`

The folder to move the project into

### importPath

Type: `string`

The new import path to use in the tsconfig.base.json

### projectName

Alias(es): project

Type: `string`

The name of the project to move

### updateImportPath

Default: `true`

Type: `boolean`

Should the generator update the import path to reflect the new location?
