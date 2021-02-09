# Monitoring internet bandwidth

* Running `influxdb` - `docker run -p 8086:8086 -v $PWD:/var/lib/influxdb influxdb`
* Running Grafana - `docker run --name=grafana -p 3000:3000 grafana/grafana`
* Running the script - `python3 script.py` (pip install -r requirements.txt)

# Running SSL Certificate checker

* Running grafana (Same as above)
* Running prometheus - `docker run --name=prometheus -p 9090:90909 -v $PWD/prometheus:/config prom/prometheus --config.file /config/prometheus.yml`
* Running Blackbox exporter - `docker run --name=blackbox -p 9115:9115 -v $PWD/blackbox:/config prom/blackbox-exporter`

## Resources used

* Taken and tweaked from https://gonzalo123.com/2018/11/26/monitoring-the-bandwidth-with-grafana-influxdb-and-docker/
* Prom with Blackbox exporter - https://geekflare.com/monitor-website-with-blackbox-prometheus-grafana/
