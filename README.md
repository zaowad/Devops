# Devops

## HW4
### Part1- implementation of link command
##### Docker file for the first app that will recieve the json
![imghw1-1](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/Dockerfile_of_application_recieving_the_json_containing_numbers_to_add_1.png)
##### pyhton application file(app1.py) for the first app that will recieve the json
![imghw1-2](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/application_receiving_the_json_2.png)
##### Docker file for the second app that will recieve a json from first app and return the sum of the two numbers inside the json dictionary
![imghw1-3](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/Dockerfile_of_second_app_3.png)
##### pyhton application file(app2.py) for the second app
![imghw1-4](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/application_recieving_the_digits_adding_them_and_sending_back_the_result_to_app1_4.png)
##### First we will build the image of the second app and run a container from this. We will do it before running a container for the first app as the second app will be linked to the first app.
![imghw1-5](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/building_the_second_app_5.png)
![imghw1-6](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/running_the_second_app_beforehand_bcz_it_will_be_linked_to_the_first_app_6.png)
##### Building and running container for the first app. While creating the container we will use link command to add an alias for the second app's container to this one.
![imghw1-7](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/building_the_first_app_7.png)
![imghw1-8](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/running_the_first_app_by_linking_it_to_the_first_app_using_the_alias_second_8.png)
##### Sending request from the server host namespace
![imghw1-9](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/sending_request_from_server_host_namespace_9.png)
### part2- load ballancing
##### Python apllication file(app1.py) for the first app
![imghw2-1](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/class_04_hw_part2_1.png)
##### Dockerfile for first app
![imghw2-2](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/class_04_hw_part2_2.png)
##### Python application file(app2.py) for the second app
![imghw2-3](https://github.com/zaowad/Devops/blob/main/devops-ss/class_04/class_04_hw_part2_3.png)
