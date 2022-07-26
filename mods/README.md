# Tribes mods

Each directory here is a full Tribes mod.

If you cloned this repo and the mod directories here are empty:
* To download _all_ mods: `git submodule update --init --recursive` (may take a while)
* To download a _single_ mod: `git submodule update --init theModDir`

## Layout

## Contributing

To contribute a new mod, first upload it to your _own_ repo (on GitHub or elsewhere). Then, submit a PR to link that
repo here as a "git submodule". See tutorials online for working with git submodules (e.g., https://chrisjean.com/git-submodules-adding-using-removing-and-updating/).

Quick guide (for each case, start from this `mods` directory):

**To add a new submodule repo:** `git submodule add git@github.com:yourAccount/yourRepo.git yourModDir` (creates new directory `yourModDir` linked to your repo)

**To update a submodule repo to a newer version:**
1. Change into the mod's directory
2. Use `git fetch` / `git pull` / etc. like you normally would to check out the newer version
3. Change back to this `mods` directory
4. `git add yourModDir`
5. `git commit ...`

Every mod directory contributed _must_ be laid out like a Tribes directory, so it can be copied over a base Tribes setup to install.

Mod directories are _recommended_ to omit base Tribes files, such as `Tribes.exe`, standard `base` content, and so on.
This keeps the repo clean and facilitates installing compatible mods together. This is not _required_, though.
