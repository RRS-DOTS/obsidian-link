# obsidian-link

Jira Cloud does not render links with the scheme `obsidian://`. This page turns an `https` link into an `obsidian://open` link, so that a note of the DOTS team vault can be opened from a Jira issue with one click.

## Use

```
https://rrs-dots.github.io/obsidian-link/?file=<path of the note>
```

`file` is the path of the note from the root of the team vault, without the extension `.md` and URL-encoded. Example:

```
https://rrs-dots.github.io/obsidian-link/?file=01%20-%20Requirements%20Management%2FAuSy%20Remote%20Control%2F00%20-%20Epic%20Summary
```

The link contains no vault name. Obsidian opens the note in the vault that is active and resolves the path like a wikilink. The browser asks once whether it may open Obsidian.

## Scope

The page only builds `obsidian://open` links. It cannot redirect to any other address. It contains no project data. The path of a note is only part of the link.
