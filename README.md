# ʕ•ᴥ•ʔ Cub - https://cub.sh

A CLI for the Bear notes app.

Usage: cub <action> [option ...]

Currently supported actions:
  create
  edit
  help
  search
  show
  token

Use 'cub help <action>' to get action specific help.

## create

Create a new note.

Example:
  cub create

## edit

Edit an existing note. Requires a title or identifier.

Examples:
  cub edit My Note Title
  cub edit title=My Note Title
  cub edit id=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX

## help

Show help information for the given action.

Examples:
  cub help create
  cub help edit
  cub help search
  cub help show
  cub help token

## search

Search your Bear notes. Requires a term or tag. By default search will return exact matches from the note title. To include all matching notes use the --all option.

Examples:
  cub search Some search terms
  cub search term=Some search terms
  cub search tag=someTag
  cub search tag=someTag term=Some search terms
  cub search --all Some search terms

## show

Show an existing note. Requires a title or identifier.

Examples:
  cub show My Note Title
  cub show title=My Note Title
  cub show id=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX

## token

Set or display a token for accessing protected Bear information. Once a token has been set, calling this without specifying a token will display the currently set token.

Examples:
  cub token
  cub token XXXXXX-XXXXXX-XXXXXX

