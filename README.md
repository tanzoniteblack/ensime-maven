[![Bountysource](https://www.bountysource.com/badge/tracker?tracker_id=239449)](https://www.bountysource.com/trackers/239449-ensime?utm_source=239449&utm_medium=shield&utm_campaign=TRACKER_BADGE)

# ENSIME Maven Plugin

This [maven](https://maven.apache.org/) plugin generates a `.ensime` file for use with an [ENSIME server](http://github.com/ensime/ensime-server).

Report issues on the [ensime-server tracker](https://github.com/ensime/ensime-server/issues) after checking the [FAQs](https://github.com/ensime/ensime-server/issues?q=label%3AFAQ)

# Usage

## Installation

This plugin should be installed on a per user basis (each user should have the option to use ensime without bloating the project definition). To use it, add the plugin to your `~/.m2/settings.xml`:

```xml
<?xml version="1.0"?>
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
          xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                              http://maven.apache.org/xsd/settings-1.0.0.xsd">
  <pluginGroups>
    <pluginGroup>st.happy_camper.maven.plugins</pluginGroup>
  </pluginGroups>
</settings>
```

## Generate `.ensime` file

Run the command `mvn ensime:generate` in the project's root directory.
