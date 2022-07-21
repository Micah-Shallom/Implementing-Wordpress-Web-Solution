# Implementing-Wordpress-Web-Solution

## STEP1 Preparing Web Server

- Create a EC2 instance server on AWS 

- On the EBS console, create 3 storage volumes for the instance. This serves as additional external storage to our EC2 machine
![created_volumes](./img/2.created_volumes.jpg)

- Attach the created volumes to the EC2 instance 
![attach](./img/3.attached_volumes.jpg)

- SSH into the instance and on the EC2 terminal, view the disks attached to the instance. This is achieved using the `lsblk` command.
![show_attached_disks](./img/4.show_attached_disks.jpg)


To see all mounts and free spaces on our server
![displaying_mountpoints](./img/5.displaying_mountPoints.jpg)

Create single partitions on each volume on the server using `gdisk `
![creating_partitions](./img/6.creating_partition.jpg)
![partitioned](./img/7.partitioned.jpg)


