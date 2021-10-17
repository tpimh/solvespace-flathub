# SolveSpace Flatpak

This is an attempt to package [SolveSpace](http://solvespace.com/) into a [Flatpak](https://flatpak.org/).

The most valuable parts are borrowed from other Flatpaks published in Flathub:

- gtkmm from [org.synfig.SynfigStudio](https://github.com/flathub/org.synfig.SynfigStudio/blob/de2fb52771d8fc30dddcec733ceb29fbf864cadc/org.synfig.SynfigStudio.yaml#L25)
- libspnav from [org.freecadweb.FreeCAD](https://github.com/flathub/org.freecadweb.FreeCAD/blob/614f56a2e88dfc27356024df3b40fae895435072/org.freecadweb.FreeCAD.yaml#L164)
- json-c from [org.fcitx.Fcitx5](https://github.com/flathub/org.fcitx.Fcitx5/blob/1c54fe416ae483cc44cbc4b7609af243f42033cd/modules/json-c.yaml)

## Building and running

```
flatpak install flathub org.gnome.Platform//3.38 org.gnome.Sdk//3.38
flatpak-builder --user --install build-dir com.solvespace.SolveSpace.yml
flatpak run com.solvespace.SolveSpace
```
