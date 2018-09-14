**How To Use:**
---------------
    
*Step 1.* Install a MySQL service by the daemon, or using the Docker installation.

*Step 2.* Build the ARA Docker image.

> $ cd ara

> $ sudo docker build -t="<path>/<image_name>" .

*You can modify the Dockerfile by you needs before you doing the docker build.*

*Step 3.* Start a Docker container for the ARA.

> $ sudo docker run --name ara -p 80:80 -e "ARA_DATABASE=mysql+pymysql://ara:password@<MySQL_Host_IP_or_FQDN>/ara" <path>/<image_name>


