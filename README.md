# waves-docker
Docker Repo for Waves.

## Usage Instructions

**Mandatory Requirement**: Must use a local mount volume and config file.

Example:

```
sudo docker run -it --name=waves-docker \   
-v /path/to/local/waves/dir:/root/waves \   
-p 127.0.0.1:6869:6869 nakuljoseph/waves-docker:latest
```

**Config file is read from**: `/root/waves/waves.conf`, i.e., `/path/to/local/waves/waves.conf`

##Storing of Data

You can store data within `/root/waves/data`.

This will inturn store your data within `/path/to/local/waves/data` described above.
