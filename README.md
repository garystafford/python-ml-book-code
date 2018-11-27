# Code for 'Python Machine Learning - Second Edition'

## Set-up

1.  `git clone` this project from GitHub
2.  Pull latest image:  `docker pull jupyter/all-spark-notebook`
3.  Deploy Docker Stack: `docker stack deploy -c stack.yml python-ml`

## Misc. Commands

```bash
docker stack ps python-ml --no-trunc
docker logs $(docker ps | grep _pyspark | awk '{print $NF}')

docker stats --format "table {{.Name}}\t{{.CPUPerc}}\t{{.MemUsage}}\t{{.MemPerc}}"

apt-get update -y && apt-get upgrade -y
apt-get install htop
htop --sort-key help
htop --sort-key
```

## References

-   [Advanced Jupyter Notebook Tricks — Part I](https://blog.dominodatalab.com/lesser-known-ways-of-using-notebooks/)
