# Big data - sampledata plugin for Joomla

Plugin that generates random content: one category (per run) with articles (10 per step), and (when enabled) menu item and custom fields for each article. Can be run multiple times.

### Build the plugin

Install:
```
phing -f build.xml build_install -Dserverpath="./web-root"
```

Final:
```
phing -f build.xml build_release -Ddestination="./output"
```
