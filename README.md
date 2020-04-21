# Portainer

Portainer is a simple management solution for Docker.

Its a web UI that allows you to easily manage your Docker containers, images, networks and volumes.

# How to deploy

Simply run the setup script from this repository. And access the port 9000 on server where Portainer is running

#  Agent

Containers, volumes, network and images are node specific resources, not cluster aware. To access one have to send query to specific node.

Agent avoids the trouble to send queries to node to access resource as it is cluster-aware. It collect all the resources available in cluster.
We have to send one API request to agent and its done.

To deploy agent we need docker swarm. Enter the following command to start docker-swarm

            docker swarm init

After its done, run the  agent script

            sh agent




