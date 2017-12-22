## FloydHub

[Quick Start](https://docs.floydhub.com/getstarted/quick_start/)

Install:

    pip install -U floyd-cli

May be needed:

    sudo pip install -U pip
    sudo apt update
    sudo apt install python-dev

init project:

    mkdir cifar
    floyd init cifar

workflow:

    floyd run "ls > /output/stdout"
    floyd logs efcic/projects/cifar/1
    floyd data clone efcic/projects/cifar/1/output

**Ref:**    
[Run a Job](https://docs.floydhub.com/guides/run_a_job/#command_1)  
[Storing Output](https://docs.floydhub.com/guides/data/storing_output)