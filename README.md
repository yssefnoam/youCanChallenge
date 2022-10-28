## My Solution for [NextMediaMa Coding Challenge](https://github.com/NextmediaMa/coding-challenges/tree/master/DevOps%20Engineer) Coding challenge II: Save our deploy train

### Overview

<img width="1338" alt="Screen Shot 2022-09-23 at 11 40 18 AM" src="https://user-images.githubusercontent.com/36737715/191944112-83befdbb-b039-49a1-9df4-c9745547ba8b.png">

### Tools:
 * [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
 * [docker and docker-compose](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04)

### Usage:
  * Clone this Repo.
  * cd youCanChallenge/
  * Run production environment:
    ```
    ansible-playbook production_env.yaml
    ```
  * Run test environment:
    ```
    ansible-playbook test_env.yaml
    ```
  
### Production_env: 
  * To test this run:
    * test 1:
    ```
      curl --header 'Host: test1.testycan.shop' localhost:8000
    ```
    * test 2: 
    ```
      curl --header 'Host: test2.testycan.shop' localhost:8000
    ```
    * test 3:
    ```
      curl --header 'Host: test3.testycan.shop' localhost:8000
    ```
### Test_env: 
  * To test this run:
    * test 1:
    ```
      curl --header 'Host: test1.testycan.shop' localhost:80
    ```
    * test 2: 
    ```
      curl --header 'Host: test2.testycan.shop' localhost:80
    ```
    * test 3:
    ```
      curl --header 'Host: test3.testycan.shop' localhost:80
    ```
