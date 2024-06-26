# Visual Studio Code user snippets

## Setup

1. Open command palette (`F1` / `Ctrl + Shift + P`)
2. Find and select `Snippets: Configure User Snippets`
3. Choose file with `.json` extension from repository

> Referenced docs:
> <https://code.visualstudio.com/docs/editor/userdefinedsnippets>

## Table of contents

| Files                                      |
| ------------------------------------------ |
| [`dockercompose.json`](#dockercomposejson) |

## Snippets

### `dockercompose.json`

#### PostgreSQL Docker container

- Create `docker-compose.yml` or `compose.yml` file
- Run snippet
- Set **name** in this line: `name: &name <<name>>`
  > Database will be available on `localhost:5432`:
  >
  > - Database: `docker`
  > - User: **name**
  > - Password: **name**
  > - Schema: **name**
- All `*.sql`files in compose file directory will be executed after database start
