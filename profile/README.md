# GAMA Community Plugins

This organisation contains all community-maintained plugins for the [GAMA platform](https://gama-platform.org). Each repository is an independent plugin with its own CI pipeline that publishes to a shared update site.

---

## Installing plugins

Open Eclipse/GAMA and go to **Help → Install New Software**, then add this update site:

```
https://updates.gama-platform.org/plugin/YYYY-MM/
```

Replace `YYYY-MM` with the GAMA version you are running (e.g. `2025-06`). All available plugins will appear in a single installable list.

> No build tools required. You do not need to clone anything to install plugins.

---

## Plugin repositories

| Repository | Plugins |
|---|---|
| `gama.plugin.inrae` | Argumentation, Bayesian Networks, IFC file, Image Analysis, QR Code, Webcam, Weka |
| `gama.plugin.irit` | CIM, Fuzzy Logic, MATLAB connector, NetCDF, Switch Project |
| `gama.plugin.femtost` | Camisole (APSF soil), Gaming, Remote GUI |
| `gama.plugin.across-lab` | PMML, Flooding simulation |
| `gama.plugin.genstar` | GenStar synthetic population |
| `gama.graphical.modeling` | Graphical/diagram modeling UI |
| `gama.plugin.mcp` | Model Context Protocol integration |
| `gama.plugin.legacy` | Archived plugins kept for reference (GamPy, Hydro, RJava, UML, …) |

---

## Creating a new plugin

1. Create a new repository in this org **from the [`gama.plugin.template`](https://github.com/gama-platform-plugin/gama.plugin.template) template**.
2. Go to **Actions → Initialize plugin from template → Run workflow** and fill in the plugin bundle ID (e.g. `gama.plugin.flooding`) and a human-readable name.
3. Pull the init commit locally, open the project in Eclipse, and start coding.
4. Push to the default branch — CI builds and publishes your plugin automatically.

See the [`gama.plugin.template`](https://github.com/gama-platform-plugin/gama.plugin.template) repository for full instructions.
