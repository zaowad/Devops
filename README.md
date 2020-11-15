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
