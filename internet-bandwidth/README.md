# Monitoring internet bandwidth

* Running `influxdb` - `docker run -p 8086:8086 -v $PWD:/var/lib/influxdb influxdb`
* Running Grafana - `docker run --name=grafana -p 3000:3000 grafana/grafana`
* Running the script - `python3 script.py` (pip install -r requirements.txt)

## Resources used

* Taken and tweaked from https://gonzalo123.com/2018/11/26/monitoring-the-bandwidth-with-grafana-influxdb-and-docker/
