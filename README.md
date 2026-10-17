# Evil Sweeper Flatpak

Signed x86_64 Flatpak repository, built and published from an Amp orb.

```sh
flatpak remote-add --user --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
flatpak remote-add --user --if-not-exists evil-sweeper https://rosenk.github.io/evil-sweeper-flatpak/evil-sweeper.flatpakrepo
flatpak install --user evil-sweeper io.github.rosenk.EvilSweeper
flatpak run io.github.rosenk.EvilSweeper
```

Updates: `flatpak update --user io.github.rosenk.EvilSweeper`.
Requires a graphical Linux session with X11 or XWayland and OpenGL 3.3.
The application has graphics/audio and device access for game controllers,
but no network or host filesystem access. All-device access supports Flatpak 1.14,
which does not have the narrower input-device permission.
The runtime is org.freedesktop.Platform 25.08, provided by Flathub.
This repository contains distributable game binaries, not the private source project.
Never replace the signing key or commit private signing material here.
