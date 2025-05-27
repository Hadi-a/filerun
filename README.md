Steps:

1. Copy Docker compose file
2. Create directories to mount volumes 

        => mkdir /filerun /filerun/html /filerun/user-files /filerun/db

3. Download the zip file from the filerun client portal.
4. Upload and extract the zip content to this path " /filerun/html "
5. Change the folder permissions to be writable by FileRun by the below cmd (to check and confirm permission, you can use cmd ls -al)

       => chown www-data:www-data -R /filerun/html/system/data 

6. Now start the Docker container by running this cmd 

      => docker compose up -d
