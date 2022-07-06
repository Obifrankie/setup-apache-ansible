This CI script is writing in yaml

This script automates the build of a apache server and hosts a html file on the server

It main point of entry is the main.yml file

It has a 2 workflows/tasks which are the
-apache
-prepare

The apche work flow setups up an apache server
The path of the apache workflow is roles/apache/tasks/main.yaml

The prepare work flow handles depenedencies
The path of the apache workflow is roles/prepare/tasks/main.yaml

To run this script localy ensure that you have ansile configured locally by running the show command python3 -m pip show ansible

and run the script with the following command ansible-playbook main.yml
