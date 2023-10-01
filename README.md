# Easy Docker for WordPress
This repo is an easy way to start a local enviroment for your WordPress development. It has a bunch of commands, inside bin folder, that can start, stop ore remove the containers, install WordPress or create a new theme (from _s or a blank one).
The environment consists of several services, including WordPress, MySQL, PHPMyAdmin, and WP CLI. It is designed to streamline WordPress development.


## Env variables
Edit the env file with you desired variables. If you want to use some of the blank ones uncomment the correspondig one in the docker-compose.yml file


## Commands
In this section, we will explain how to use the provided scripts and commands.

`bin/start` Start the enviroment

`bin/stop` Stop all the container

`bin/stop` Stop and remove all the container


`bin/install` Install WordPress using .env for admin username, password and email


`bin/cli` You can pass any command that you want to use with WordPress cli. EX. `bin/cli --info`


`bin/theme` This script simplifies theme management in your WordPress development environment. Use it without parameters to display the helper function. It provides the following functionality:

&ensp;**Theme Creation (create):** You can generate a new theme based on the _s (Underscores) starter theme by providing a theme name and author.

&ensp;**Blank Theme Creation (blank):** This command creates a blank WordPress theme with the specified slug and author. It includes essential theme files and initializes the style.css file with theme metadata.

&ensp;**List Installed Themes (list):** Use this command to list all the themes installed in your WordPress environment.

&ensp;**Theme Activation (activate):** You can activate a specific theme by providing its name as an argument.