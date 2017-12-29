## Data

This part of code will get training data used by RL algorithm.

## Real Data

Run `sudo python3 real_data.py` and the real throughput will be written in `net_data.txt`.

## Synthetic Data

Run `python3 synthetic.py` to get some synthetic data, both stable and unstable throughput are included.

## Get Dataset

If you need a large dataset to train your model, maybe you can try the following commands.

```
# FCC broadband dataset
$ wget http://data.fcc.gov/download/measuring-broadband-america/2016/data-raw-2016-jun.tar.gz
$ tar -xvzf data-raw-2016-jun.tar.gz -C fcc

# Norway HSDPA bandwidth logs
$ wget -r --no-parent --reject "index.html*" http://home.ifi.uio.no/paalh/dataset/hsdpa-tcp-logs/

# Belgium 4G/LTE bandwidth logs (bonus)
$ wget http://users.ugent.be/~jvdrhoof/dataset-4g/logs/logs_all.zip
$ unzip logs_all.zip -d belgium
```