Hi, I’m Artur.  
At work I am helping software teams to grow and build their engineering excellence.  
Currently trying to give back to open source and working on [Salix](https://github.com/artursulkowski/salix) project.

## Mini Blog

### Added starlark script to [ansible-pi-pub](https://github.com/artursulkowski/ansible-pi-pub)
<sup>2023.04.24, Artur</sup>  
I use Shelly3EM as energy meter. Shelly measures power separately for each phase.  
I needed to summarize power measurement from each phase as they are received over MQTT.  
[Starlark](https://github.com/influxdata/telegraf/blob/release-1.26/plugins/processors/starlark/README.md) become very handy as within telegraf I could capture measurements, calculate summary power and send it back over MQTT.  
You can find details in [telegraf.conf](https://github.com/artursulkowski/ansible-pi-pub/blob/main/roles/telegraf/files/telegraf.conf)

[Some extra reading about starlark](https://www.influxdata.com/blog/how-use-starlark-telegraf/)

<!---
artursulkowski/artursulkowski is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
