# Initialize

Clone repository:
```console
chezmoi cd
chezmoi init git@github.com:magic0whi/proteus_dotfiles.git
```

See what would be changed:
```console
chezmoi diff
````

Edit and errors...

# Concepts

- Destination directory: `~/`

  Destination Stage: `&destination_directory`
- Source directory: `~/.local/share/chezmoi/`

  Source state: `&source directory`
- Target directory: `~/`

  Targe state: `~/` after `chezmoi apply`
- Working tree `~/.local/share/chezmoi/`

# Daily operations

Show diff & summary:

```console
chezmoi diff
chezmoi status
```

Update from source directory:
```console
chezmoi -v apply
```

Update from destination:

```console
chezmoi re-add filename
```

Convert to template:

```console
chezmoi chattr +template filename
```

Revert from template (Only filename changed):

```console
chezmoi chattr -- -template filename
````

List chezmoi managed files:

```console
chezmoi managed
```

List template data (environment vaiable):

```console
chezmoi data
````
