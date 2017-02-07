# Wordcamp Extension Beta
Adds WordCamp support to Chassis

This is based on [meta-environment](https://github.com/WordPress/meta-environment) by Automattic.

## Installing & Documentation

1. Clone chassis `chassis` by `git clone --recursive https://github.com/Chassis/Chassis chassis`.
2. Download the `config.yaml` - [config template](https://gist.github.com/stuartshields/7673027fa016506d29e061a788a1bde6) and paste it into the `/vagrant` folter (this will overwrite the existing file)
3. Add the following to your `hosts` file
	1. `10.86.73.80 wordcamp.dev`
	2. `10.86.73.80 central.wordcamp.dev`
	3. `10.86.73.80 2014.new-site.wordcamp.dev`
	4. `10.86.73.80 2014.content.wordcamp.dev`
	5. `10.86.73.80 2014.misc.wordcamp.dev`
	6. `10.86.73.80 2014.seattle.wordcamp.dev`
	
4. `vagrant up`
5. `git clone git@github.com:stuartshields/chassis-wordcamp.git extensions/vip`
6. `vagrant provision` - Depending on your internet connection, this could take a while

### Adding additional extensions
It's recommended that you install the following Chassis extensions

[PHPCS & WPCS](https://github.com/Chassis/phpcs)

[Memcache](https://github.com/Chassis/memcache)

[Debugging](https://github.com/Chassis/Debugging)

Once all extensions are added you can now `vagrant provision`
