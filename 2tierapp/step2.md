Kustomization.yaml file generates the secrets for the mysql root password
`cat kustomization.yaml`{{execute}}

The following manifest describes a single-instance MySQL Deployment. The MySQL container mounts the PersistentVolume at /var/lib/mysql. The MYSQL_ROOT_PASSWORD environment variable sets the database password from the Secret
`cat mysql-deployment.yaml`{{execute}}

MySQL and Wordpress each require a PersistentVolume to store data. Their PersistentVolumeClaims will be created at the deployment step
