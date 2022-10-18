- Run upgrade `sudo apt-get upgrade -y`
- check internet conectivity  `sudo apt-get update`
- Run upgrade `sudo apt-get upgrade -y`
- where am i `pwd`
- `whoami`-folder name, `uname`-gives OS used in vm or `uname -a` - version of $
- how to create a file in linux `touch 'filename'` & `nano filename`
- check files available in current location - `ls`
- navigate to folder `cd folder name`
- how to navigate out of folder `cd..` or `cd` enter
- how to delete a file/foldername' research how to copy file from 1 location to$
- copy test.txt into app folder
- how to navigate between os & vm `exit` enter
- for admin access `sudo` switch to admin user `sudo su`
- change permission `chmod instructions file-name` i.e `chmod 700 test.txt`
- currently running process `top`
- currently running process `top` & `ps aux`
- to remove any process `kill "PID"` - `kill 7`
- how to delete folder/hidden folder `la -a`



# exercise
- print last 3 lines from the test.txt
`tail -3 test.txt`
- print first 3 lines from the test.txt
`head -3 test.txt`
- print last 10 lines from the test.txt
`tail -10 test.txt`
- print last lines from the test.txt
to print from the bottom you would use `tail -n [value] filename`
- research how to use `| pipe` & ` grep` & `sort`
- - `pipe` command lets you sends the output of one command to another. Piping, as the term suggests, can redirect the standard output, input, or error of one process to another for further processing.
- - The `grep` filter searches a file for a particular pattern of characters, and displays all lines that contain that pattern.
- - `SORT` command is used to sort a file, arranging the records in a particular order. 
- `ps aux` short list by name
- - The `ps aux` command is a tool to monitor processes running on your Linux system.
- How to create/run a process in the background & foreground, create/run a process in both areas
- kill the process that you created


- install `nginx` in our vm
- create an IP address - for mac users
- `sudo apt-get install nginx -y`
- how to check a tool/software status in linux `sudo systemctl status nginx`
- how to restart a process in linux 
- mac ip ranges `192.168.56.10` `192.168.56.11` `192.168.56.12`
- how to check a tool/software status in linux `sudo systemctl status [name]`
- how to restart a process in Linux `sudo systemctl start [name]`, `sudo systemctl stop [name]` `sudo systemctl start [name]`
- need to put private network in vagrant file
- added `config.vm.network "private_network", ip: "192.168.56.0"` to vagrant file
- then done `vagrant reload` on local host terminal
- used `vagrant ssh` to get back in
- if `vagrant reload` doesn't work then try `vagrant destroy` and then `vagrant up`
- `sudo systemctl stop nginx` stops process
- `sudo systemctl start nginx` starts process


/Users/maiza/eng130_virtualisation/images/dev_eng


# What is virtualisation
Virtualization is technology that lets you create useful IT services using resources that are traditionally bound to hardware. It allows you to use a physical machine’s full capacity by distributing its capabilities among many users or environments.

## Benefits of virtualisation
1. Slash your IT expenses
- Utilizing a non-virtualized environment can be inefficient because when you are not consuming the application on the server, the compute is sitting idle and can't be used for other applications. When you virtualize an environment, that single physical server transforms into many virtual machines.

2. Reduce downtime and enhance resiliency in disaster recovery situations
- When a disaster affects a physical server, someone is responsible for replacing or fixing it—this could take hours or even days. With a virtualized environment, it’s easy to provision and deploy, allowing you to replicate or clone the virtual machine that’s been affected. The recovery process would take mere minutes—as opposed to the hours it would take to provision and set up a new physical server—significantly enhancing the resiliency of the environment and improving business continuity.

3. Increase efficiency and productivity
- With fewer servers, your IT teams will be able to spend less time maintaining the physical hardware and IT infrastructure. You’ll be able to install, update, and maintain the environment across all the VMs in the virtual environment on the server instead of going through the laborious and tedious process of applying the updates server-by-server. Less time dedicated to maintaining the environment increases your team’s efficiency and productivity.

# What is vagrant
Vagrant is an open-source tool that helps us to automate the creation and management of Virtual Machines. In a nutshell, we can specify the configuration of a virtual machine in a simple configuration file, and Vagrant creates the same Virtual machine using just one simple command. It provides command-line interfaces to automate such tasks. 

# What is virtual box
VirtualBox is open-source software for virtualizing the x86 computing architecture. It acts as a hypervisor, creating a VM (virtual machine) in which the user can run another OS (operating system). The operating system in which VirtualBox runs is called the "host" OS. The operating system running in the VM is called the "guest" OS

# Why should we use them all
Building a software prototyping environment (aka lab) is far simpler than ever before. No longer do you have to wait to build a physical machine, then wait to download ISO images of the virtualization stuff, operating systems, software packages etc.
Simply use Vagrant and VirtualBox together. You'll have a highly functional lab for software development up fast with some added agility for prototyping infrastructure choices too.