# kurseve Ansible OpenCV 3 playbook

Ansible playbook for provisioning `OpenCV 3.1.0` with `python3` on a vagrant environment

## Box info

- Ubuntu 14.04.5 LTS
- RAM: 2GB
- cpu: 2
- swapfiles: not created (yet)

## Setup

```sh
$ git clone https://github.com/prodicus/opencv3-ansible-vagrant-playbook.git && cd opencv3-ansible-vagrant-playbook
$ vagrant up
```

And that's it!

to check if everything went fine

```sh
$ vagrant ssh
....
vagrant@kurseve:~$ workon cv
(cv) vagrant@kurseve:~$ python
Python 3.4.3 (default, Nov 17 2016, 01:08:31)
[GCC 4.8.4] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import cv2
>>> cv2.__version__
'3.1.0'
>>>
```

## TODO

- [ ] Add shared folders inside for easy access to converted files
- [ ] Add a GUI instead of a headless vm box for ease of use

## LICENSE

GPLv3
