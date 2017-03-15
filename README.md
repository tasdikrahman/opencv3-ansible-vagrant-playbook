# kurseve Ansible OpenCV 3 playbook

Ansible playbook for provisioning `OpenCV 3.0.0` with `python2` on a vagrant environment

## Box info

- Ubuntu 14.04.5 LTS
- RAM: 2GB
- cpu: 2
- swapfiles: not created (yet)

## Setup

```sh
$ git clone https://github.com/prodicus/opencv3-ansible-vagrant-playbook.git && cd opencv3-ansible-vagrant-playbook
$ git checkout python2
$ vagrant up
```

And that's it!

to check if everything went fine

```sh
$ vagrant ssh
Welcome to Ubuntu 14.04.5 LTS (GNU/Linux 3.13.0-108-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Wed Mar 15 19:16:51 UTC 2017

  System load:  0.07              Processes:           96
  Usage of /:   3.6% of 39.34GB   Users logged in:     0
  Memory usage: 6%                IP address for eth0: 10.0.2.15
  Swap usage:   0%

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.

New release '16.04.2 LTS' available.
Run 'do-release-upgrade' to upgrade to it.


Last login: Wed Mar 15 19:39:24 2017 from 10.0.2.2
vagrant@kurseve:~$ workon cv
(cv) vagrant@kurseve:~$ python
Python 2.7.6 (default, Oct 26 2016, 20:30:19)
[GCC 4.8.4] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import cv2
>>> cv2.__version__
'3.0.0'
>>>
```

## TODO

- [ ] Add shared folders inside for easy access to converted files
- [ ] Add a GUI instead of a headless vm box for ease of use

## LICENSE

GPLv3
