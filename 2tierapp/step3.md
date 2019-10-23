The following manifest describes a single-instance WordPress Deployment. The WordPress container mounts the PersistentVolume at /var/www/html for website data files


The WORDPRESS_DB_HOST environment variable sets the name of the MySQL Service defined above, and WordPress will access the database by Service 


The WORDPRESS_DB_PASSWORD environment variable sets the database password from the Secret kustomize generated

`cat wordpress-deployment.yaml`{{execute}}
