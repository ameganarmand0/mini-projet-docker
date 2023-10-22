to test this docker project you may have:
-  docker installed
-  docker-compose installed
-  cd to simple_api folder and build api image (docker build -t studentlist:v1 .)
-  cd to mini-projet-docker folder and run => docker-compose up -d
-  open browser to test app ihm => http://<host_ip>:8300/ 
-  test your registry ui => http://localhost:8200/
-  push images to your registry
      docker tag <image_to_push_id> <registry_container_name>:<registry_container_internal_ip>/<new_name>
      docker push <registry_container_name>:<registry_container_internal_ip>/<new_name>