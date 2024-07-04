# YoungDB

**Still working in progress.**

YoungDB is a time series data storage engine that is highly optimized for SSDs, which has lower write amplification.

## Building

You can clone the InfluxDB repository from GitHub using a SSH connection:

```shell
git clone git@github.com:noorall/influxdb.git
```

or via HTTPS:
```shell
git clone https://github.com/noorall/influxdb.git
```

Currently, tsdb exists as a submodule within InfluxDB. that need to be checked out with:

```shell
git submodule update --init --recursive
```

If you want to switch the remote to your fork, you can achieve this by:

```shell
cd tsdb
git remote -v
git remote remove origin
git remote add origin <HTTPS-URL-TO-YOUR-FORK>
```

As a next step check out the tsdb branch you want to build and install:

```shell
cd tsdb
git checkout <tsdb-branch-you-want-to-use>
git config --global --add safe.directory `pwd`
```

