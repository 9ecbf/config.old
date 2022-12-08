_It contains few bash-scripts I wrote at my leisure that makes my life easier to migrate onto new Linux machines._

## Usage
Open a terminal and run the following command to load the `abc` configuration:
```
$ curl -sL $CONFIG_HOST/load | sudo bash -s abc
```
To load more configurations, just pass the name of which configuration you need after the `-s` in the above command. The available configurations (`.conf` files) could be seen [here](/.config). Remember that the configuration's name mustn't contain the suffix `.conf`.

To install `xyz`, run:
```
$ curl -sL $CONFIG_HOST/install/xyz | sudo bash
```

A script `jqk` from my [scripts](.bin) could be installed by executing:
```
$ curl -sL $CONFIG_HOST/install/bin | sudo bash -s jqk
```

After all, to load all changes into your login session, use this command:
```
$ source ~/.bashrc
```

_Note:_
The `$CONFIG_HOST` is where you can fetch the scripts. You can use `https://raw.githubusercontent.com/9ecbf/config/master` (this repository), or use `https://config.tuanm.dev` for short. You should set it as an environment variable before running the commands for more convenience:
```
$ export $CONFIG_HOST=https://config.tuanm.dev
```


**Hope you enjoy the scripts. Use them at your own risk!**
