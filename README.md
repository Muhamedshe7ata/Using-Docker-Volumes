# Using-Docker-Volumes>

To change the name of a volume in Docker, you can use the following steps:

Stop the container that is using the volume:
docker stop <container_name_or_id>
2- Remove the container:
docker rm <container_name_or_id>

3-Remove the volume with its original name:
docker volume rm <original_volume_name>

4-docker volume rm <original_volume_name>

docker volume create --name <new_volume_name>

5-
Run a new container, mounting the new volume and mapping it to the same directory as the original volume:
docker run -d -v <new_volume_name>:<mount_point> <image_name>
This will launch a new container with the specified Docker image, using the newly created volume and mapping it to the same mount point as the original volume.

Form more info plz visit:
https://www.youtube.com/watch?v=5cujpTjGXFc&list=PLX1bW_GeBRhDkTf_jbdvBbkHs2LCWVeXZ&index=17&ab_channel=Codographia

