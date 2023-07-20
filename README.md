Hi, I’m Artur.  
At work I am helping software teams to grow and build their engineering excellence.  
Currently trying to give back to open source and working on [Salix](https://github.com/artursulkowski/salix) project.

## Mini Blog


### First version of charging controller ### 
<sup>2023.07.20, Artur</sup>  
Quite a good progress over last few weeks and first version of [Charging Controller](https://github.com/artursulkowski/slxchargingcontroller) is ... almost ready. It is working functionally on development environment with HA 2023.05. It requires few tweaks to be [compatible with HA 2023.07](https://github.com/artursulkowski/slxchargingcontroller/issues/17). After this is done I can switch to "UAT" testing in my home installation. 

One big news from 2023.07 release is [introduction of responses to services](https://www.home-assistant.io/blog/2023/07/05/release-20237/?ref=building.open-home.io#services-can-now-respond) . This will allow me to easier connect [SLX Charging Controller](https://github.com/artursulkowski/slxchargingcontroller) with other Salix integrations (like charging planner).

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
