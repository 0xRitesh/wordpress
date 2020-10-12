## wordpress

This is a WordPress repository configured to run on the Pantheon platform.
this is website platform optimized and configured to run high performance sites with an amazing developer workflow.

This repository is an under reconstruction wordpress project that can be used to start a new website. It also contains some tools to help project industrialisation (deployment, testing, content manipulation...).

## Create a new project
To start a new project using this barebone one, you just need to run :

composer create-project chstudio/wordpress-project [path] [version]
[path] is the path to the installation directory, if not defined, a wordpress-project folder will be created in your current path.
[version] is the version of the project to use when installing, if not defined, the more recent stable is used, else you can use : dev-master, v0.0.0, ...
You can also use a simple git clone :

git clone https://github.com/wordssaysalot/wordpress.git


## Installation
This project rely on WP-CLI to perform common tasks.

To install your local environment you must run the following commands :

bin/wp core download
bin/wp core config
bin/wp core install
mv public/wp-cms/wp-config.php public
If your local configuration is not defined, you must pass all the required parameters. You can get more details by running --help flag on each command (will display parameters and command description).

If you haven't defined it, the core install will prompt the generated administrator password, you'll be asked to change it after your first admin panel login.

The last one moves the generated configuration file to your project public root. It's mandatory to use the public/wp-content folder as code container.

When the execution has succeded, you can access your local installation.


## Contributing
We welcome everyone to contribute to this project. Below are some of the things that you can do to contribute.

Read our contributing guide.
Fork us and request a pull to the develop branch.
Submit bug reports or feature requests to GitHub.

#License

GPL-3.0 License
