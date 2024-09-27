# Big data - sampledata plugin for Joomla

Joomla plugin that generates random content: one category (per run) with articles (10 per step), and (when enabled) menu item and custom fields for each article. Can be run multiple times.

By default it has 221 steps which will generate 1 category and around 2k articles, and 2k menus (when enabled), in one run, 2 run will produce ~4k articles, 3 run ~6k and so on.
It is possible to set 500 steps (and more), however it may actually slow down MySQL, and take longer than when the sample data executed twice.

Additionally, to speed up sample data creation need to disable "Content - Smart Search" and "Behaviour - Versionable" plugins.


### Build the plugin

Install:
```
phing -f build.xml build_install -Dserverpath="./web-root"
```

Final:
```
phing -f build.xml build_release -Ddestination="./output"
```
