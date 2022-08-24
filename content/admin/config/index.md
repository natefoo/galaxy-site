---
title: Galaxy Configuration for Admins
---

<slot name="/admin/linkbox" />

## Production Galaxy

* [Running Galaxy in a production environment](https://docs.galaxyproject.org/en/latest/admin/production.html)
* [Running Galaxy Tools on a Cluster](https://docs.galaxyproject.org/en/latest/admin/cluster.html)
* [Galaxy Job Configuration](https://docs.galaxyproject.org/en/latest/admin/jobs.html)
* [Authentication with LDAP/AD](/admin/config/external-user-auth/)
* [Apache Proxy](https://docs.galaxyproject.org/en/latest/admin/special_topics/apache.html)
    * [Apache External User Auth](/admin/config/apache-external-user-auth/)
* [Nginx Proxy](https://docs.galaxyproject.org/en/latest/admin/special_topics/nginx.html)
    * [Nginx External User Auth](/admin/config/nginx-external-user-auth/)

## Tools

* [Tool Dependencies](/admin/config/tool-dependencies/)
* [Set up Visualizations](/visualization-setup/)
* [Collecting Job Metrics](https://docs.galaxyproject.org/en/latest/admin/special_topics/job_metrics.html)


## tusd

* [Performant Uploads with TUS](https://training.galaxyproject.org/training-material/topics/admin/tutorials/tus/tutorial.html)
* [The galaxy-upload command line upload utility](https://galaxy-upload.readthedocs.io/)

## FTP

NOTE: TUS provides robust, resumable uploads via the UI, API, and command line with little-to-no effort and is
recommended over FTP for Galaxy servers running 22.01 or later.

* [Upload via FTP](https://docs.galaxyproject.org/en/latest/admin/special_topics/ftp.html)
* [Setup ProFTPd with AD/LDAP auth](/admin/config/proftpd-with-ad/)

## Other

* [User Information (Collecting information during registration)](/admin/config/user-information/)
* [Running on Windows](/admin/config/windows/)
* [Access Control (ACLs)](/admin/config/access-control/)
