This CI script is writing in yaml

This playbook automates the build of a apache server and hosts a html file on the server

It main point of entry is the main.yml file

It has a 2 workflows/tasks which are the
-apache
-prepare

The apche play setups up an apache server
The path to the apache play is roles/apache/tasks/main.yaml

The prepare work play handles depenedencies
The path play the apache play is roles/prepare/tasks/main.yaml

To run this playbook localy ensure that you have ansile configured locally by running the show command python3 -m pip show ansible

and run the playbook with the following command ansible-playbook main.yml
