# Kibi/Kibana Radar Chart Plugin

This is a plugin for [Kibana 4.3+](https://www.elastic.co/products/kibana) and [Kibi](http://siren.solutions/kibi) (our [extention of Kibana for Relational Data](https://www.linkedin.com/pulse/extending-elasticsearch-kibana-do-data-intelligence-kibi-tummarello)) 0.3.

A radar chart is a graphical method of displaying multivariate data in the form of a two-dimensional chart of three or more quantitative variables represented on axes starting from the same point. The relative position and angle of the axes is typically uninformative.

![image](img/radar.png)
![image](img/kibana.png)

## Installation

This plugin can be installed in both:
 
 * [Kibana: 4.3+](https://www.elastic.co/downloads/past-releases/kibana-4-3-0)
 * [Kibi: 0.3+](https://siren.solutions/kibi) (Coming soon ...)

### Automatic

```
# for kibi
./bin/kibi plugin -i kibi_radar_vis -u  https://github.com/sirensolutions/kibi_radar_vis/archive/0.1.0.zip
# for kibana
./bin/kibana plugin -i kibi_radar_vis -u  https://github.com/sirensolutions/kibi_radar_vis/archive/0.1.0.zip
```

### Manual

```
git clone https://github.com/sirensolutions/kibi_radar_vis.git
cd kibi_radar_vis
npm install
npm run build
cp -R build/kibi_radar_vis KIBANA_FOLDER_PATH/installedPlugins/
```

## Uninstall

```
# for kibi
bin/kibi plugin  --remove kibi_radar_vis
# for kibana
bin/kibana plugin  --remove kibi_radar_vis
```

## Development

- Clone the repository at the same level of a Kibana > 4.3 clone
- If needed, switch to the same node version as Kibana using nvm 
  (e.g. `nvm use 0.12`)
- Install dependencies with `npm install`
- Install the plugin to Kibana and start watching for changes by running 
  `npm start`
