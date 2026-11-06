# Old Flurry 64 Bit — 2026 Beta

A separate Windows x64 launcher and experimental x64 DirectX 12 client.

## Download

Download **Old-Flurry-64-Bit-v3.0.0-Beta.zip** from [Releases](https://github.com/edgewoodnm/SWG-Old-Flurry-64bit/releases). Extract the ZIP completely and run `OldFlurryLauncher.exe`. Setup creates permanent Desktop and Start Menu shortcuts. Click **DOWNLOAD & INSTALL**, wait for verification, then **PLAY**.

The ZIP includes the x64 client executable, matching runtime DLLs, the self-contained x64 launcher and approved Old Flurry artwork. The launcher downloads the existing sanitized base-game archives and latest public content separately. Internet and approximately 20 GB free disk space are required. No separate .NET installation is needed.

Installed location: `%LOCALAPPDATA%/SWGOldFlurry64/Game`. The classic client remains under its existing separate folder. Players can retain either or both clients. No account passwords, profiles or owner settings are bundled. Public server defaults are generated on the player's PC.

## Patches for both clients

Both launchers consume the same public content feed:
`https://raw.githubusercontent.com/edgewoodnm/SWG-Old-Flurry-Assets/main/manifest.json`

Publish compatible content patches once there to update both 32-bit and 64-bit installations. Custom content stays in TRE archives; `client.cfg` registration remains supported. The x64 launcher preserves its final native renderer/configuration include across those shared updates.

Architecture-specific binaries remain separate. This repository's `client-runtime.json` controls only x64 executable/runtime updates. Classic executable updates remain on the classic channel. Never put DLLs or EXEs into the shared TRE feed. A patch requiring architecture-specific code must ship the corresponding binaries on each relevant channel and be tested with both clients.

Base game downloads reuse the already published sanitized base archives. This repository owns the base manifest selection; it does not duplicate their multi-gigabyte storage.

## Validation and limits

The launcher checks manifests and SHA-256 hashes before enabling Play; verifies installed content/runtime; blocks corrupt packages; creates local update backups; retains content rollback/repair handling. Every Play checks current feeds. Missing network/update verification blocks Play.

This is a beta, not a guarantee of performance or stability. Intended Windows 10/11 x64; actual Windows 10 testing remains pending. Compatible DirectX 12 hardware/drivers and Shader Model 6.0 are required. The classic x86 DXVK face-fix is not applied to the x64 DX12 client. Client gameplay testing, including the god-buff regression, audio, combat, travel and GPU coverage, remains pending. More RAM or a faster PC alone does not guarantee compatibility.

## Credits

Malakai (Final), original SWG 2.0 64-bit work; SWG-Source and upstream contributors; Old Flurry integration and fixes. Client donor commit `0dc21e65c213a429628aaf3d51f2a6625c108737`; Old Flurry client integration `b3ce9d15e`. Existing game/runtime licenses and upstream attribution continue to apply.

## Maintainers

Upload release assets as a draft, verify server-reported size and SHA-256, then publish the release and activate the matching runtime manifest. Keep public releases free of local configs, accounts, profiles, logs, private server files and credentials. Launcher source is not included in this distribution repository.


## Public content QA v1.0.35

The full Jabba rancor pit, trained mount reward, Stormtrooper Deluxe Blaster Rifle and Twin Legacy Jedi mantles are available through the existing shared content feed. Close the game and update the current launcher; no new launcher or x64 runtime is needed. Darth Maul awards both new robes and the existing saber readout. See [full QA notes](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.35).

The cumulative TRE-only ZIP was validated through both real installer implementations, including x64 final renderer include restoration, installed receipt verification, preserved personal files and all241 active resource hashes. Full group balance, species fit, crafting and wider hardware coverage remain QA. The architecture-specific runtime manifest and base archives are unchanged.


## Rancor pit loading-screen QA v1.0.36

The existing shared content updater now supplies matching rancor-pit artwork/story, preserves loading controls and separate Hoth artwork, and retains all v1.0.35 content. Close the game and update the current launcher. No launcher/runtime replacement or server restart. [Release and test notes](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.36). Native install/resource checks passed; owner in-game loading visual test is pending.


## Life Day assets and QA console v1.0.37

The existing shared content updater now supplies the Imperial Frostspire tree, seven standalone Life Day inflatables and QA house console presentation, retaining all previous content. Close the game and update the existing launcher. No launcher/runtime replacement. Server activation occurs with the warned maintenance. [Release and test notes](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.37). Native install/resource checks passed; in-game seasonal visual and console retrieval testing remain pending.


## Sally, Moonlit Mischief and Doc-1985 QA v1.0.38

The shared content updater adds Sally Stitched Wishes Inflatable, Moonlit Mischief Snow Globe and the Doc-1985 Vehicle Deed for the house QA console, retaining all previous content. Close the game and update the existing launcher. No launcher/runtime replacement. Server activation occurs with the warned maintenance. [Release and test notes](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.38). Native install/resource checks passed; in-game seasonal visual and console retrieval testing remain pending.


## Admin command visibility v1.0.39

Shared classic and x64 update registers CSR commands. Native server account permissions still control access. Close the game, update the existing launcher and relaunch. No server restart or launcher replacement. Both native updater checks passed. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.39).


## Aurora Spire city tree v1.0.40

Adds a 12-metre rainbow Life Day city tree to the QA console and both seasonal vendors for 25 tokens. Uses native mayor-only city placement. Life Day remains disabled. Shared update for classic and x64 clients; no launcher or runtime replacement. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.40). Native updater checks passed; city placement and visual gameplay QA pending.


## Vanguard speeder bikes v1.0.41

Adds Imperial and Rebel Vanguard single-seat bikes to Darth Vader for 1,000,000 credits each. Includes dual exhaust, fitted controls and the owner-confirmed mounted robe visibility repair. Life Day remains disabled. Shared update for classic and x64 clients; no launcher or runtime replacement. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.41). Native updater checks passed; Owner private riding and robe visual tests passed; broader species QA ongoing.


## Vanguard handling v1.0.42

Vanguard bikes gain base speed224, eightfold acceleration and braking70, with repaired native handling bindings. Store and recall after updating. Life Day remains disabled. Shared update for classic and x64 clients; no launcher or runtime replacement. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.42). Native updater checks passed; Owner private riding and robe visual tests passed; broader species QA ongoing.


## Galactic Beacon lightshow tree v1.0.43

Separate animated green LED tree displaying red Rebel and white Imperial emblems with sweeps and chases. Original static rainbow tree preserved. Available from the QA console; seasonal vendors ready at 25 tokens, with Life Day still disabled. Shared classic/x64 TRE-only update, no launcher or runtime replacement and no server restart. Owner confirmed private classic animation; broader rendering and placement QA ongoing. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.43).


## Old Flurry LED billboards v1.0.44

Three branded LED signs with irregular red-cloud lightning, permanent Mos Eisley starport/cantina buildout placements, and QA console items. Includes matching client buildout rows and cantina wall clearance. Shared classic/x64 TRE-only content update; launcher and runtime unchanged. Owner confirmed base sign rendering; latest storm, final clearance and broader placement/hardware QA ongoing. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.44).


## Runtime 0.1.1: desktop switching

Borderless fullscreen and Windows-key access, delivered through the existing launcher Update button. Close the game before updating, then relaunch. Configuration-only patch; binaries, graphics backend, login settings, profiles, content and base client preserved. No replacement launcher or server restart. Native installer and borderless/non-topmost window checks passed; player keyboard confirmation pending. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-64bit/releases/tag/runtime-0.1.1).


## Be Kind / Mod the Galaxy billboard v1.0.45

Adds the large bright LED billboard to the shared classic/x64 content feed and QA console. 44-second show: longer picture holds and unchanged flashing green final words. Includes the approved saved Mos Eisley world display; this client package adds no duplicate world placement. Existing x64 runtime 0.1.1 desktop-switching fix is preserved. No replacement launcher or server restart required. Broader hardware/city placement QA continues. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.45).


## Elder Jedi v1.0.46

Standalone Elder Jedi profession, classic skill training, custom ability icons, main-menu holocron training, robe milestones and three fifth-generation lightsaber recipes at level 90. Shared TRE content for both 32-bit and 64-bit launchers. Existing x64 runtime and base distribution are preserved. Crafting and balance QA continues. [Release](https://github.com/edgewoodnm/SWG-Old-Flurry-Assets/releases/tag/v1.0.46).
