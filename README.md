# ldap2ssm

Retrieves storage metrics in the grid BDII and uses them to produce StAR-SSM compliant records.

## Build

To buil the gem simply issue the command:

    gem build gem build ldap2ssm.gemspec

## Installation

Add this line to your application's Gemfile:

    gem 'ldap2ssm'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ldap2ssm
    
## Dependencies

This gem depends on the 'faustcommon' gem that you can find at:

    https://github.com/andreaguarise/sendToFaust-common

## Usage

	The command can be run with
	
	$ldapssm_run -C $confpath
	
	Usage: ldap2ssm_run [OPTIONS]
   
    -C, --Conf conf                  Path to configuration file dir
    -h, --help                       Print this screen

	The option -C allows to specify the directory containing the configuration files. 
	
## Config Files

	Two configuration files are needed. They must be in the same directory, which in turn can be specified with the -C option 
	on the command line.
	
	The file ldap2ssm.properties contains the config parameters of the script. 
	Another file usually sitelist.conf contains, one per line, the list of GOCDB name of sites for wich usage records will be produced.
	
## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
