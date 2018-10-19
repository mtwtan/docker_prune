# docker_prune
This simple script runs through all the nodes in a container platform that runs Docker containers and sets up weekly cron job to prune unused docker volumes. It is designed so that each node is given an hour starting from 12 midnight to do the necessary pruning. Each node will not be pruning at the same time to avoid any potential race condition.
