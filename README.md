# Worgoblin High Elf Common MPQ files
This repo contains the files that both the 32-bit and 256-bit versions of WHE use. Keeping these client-only files separate saves time and space.

You can clone them directly into your client's Data folder **if you don't have a conflicting** patch-A.MPQ or Optional/patch-J.MPQ there already.

`modpaks/<modpak>/` holds client files that only belong with one modpak (e.g. F-133's Mists of Pandaria world map), laid
out like a patch. Don't copy them into `patch-A.MPQ`: WHE's `deploy-dbc.sh` (with `LOCAL_COMMON_DIR` set) copies them
into the realm's own patch, `patch-A.<realm>.MPQ`, for the modpaks in that realm's manifest, and removes them again
when a modpak leaves it.
