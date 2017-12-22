## FloydHub

[Quick Start](https://docs.floydhub.com/getstarted/quick_start/)

### Install:

    pip install -U floyd-cli

May be needed (AWS Cloud9):

    sudo pip install -U pip
    sudo apt update
    sudo apt install python-dev

init project:

    mkdir cifar
    floyd init cifar

### Workflow:

Command:

    floyd run "ls"
    floyd logs efcic/projects/cifar/1

Output:

    ################################################################################
    2017-12-22 04:23:50,941 INFO - Run Output:
    2017-12-22 04:23:51,281 INFO - /code
    2017-12-22 04:23:51,330 INFO - 
    ################################################################################

Output to File:
        
    floyd run "ls > /output/stdout"
    floyd data clone efcic/projects/cifar/1/output

**DATA**

* [Upload](https://docs.floydhub.com/guides/create_and_upload_dataset/#upload-a-dataset)
* [Mount](https://docs.floydhub.com/guides/data/mounting_data/#the-data-flag)

**Ref:**    
* [Run a Job](https://docs.floydhub.com/guides/run_a_job/#command_1)
* [Storing Output](https://docs.floydhub.com/guides/data/storing_output)