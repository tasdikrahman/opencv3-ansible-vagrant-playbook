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

- [x] ~~Add `python2` support for the vagrant box.~~ Added on [python2](https://github.com/prodicus/opencv3-ansible-vagrant-playbook/tree/python2) branch.
- [ ] Add shared folders inside for easy access to converted files
- [ ] Add a GUI instead of a headless vm box for ease of use

## LICENSE

GPLv3

If you have found my little bits of software being of any use to you, do consider helping me pay my internet bills :)

## Donation

| PayPal | <a href="https://paypal.me/tasdik" target="_blank"><img src="https://www.paypalobjects.com/webstatic/mktg/logo/AM_mc_vs_dc_ae.jpg" alt="Donate via PayPal!" title="Donate via PayPal!" /></a> |
|:-------------------------------------------:|:-------------------------------------------------------------:|
| Gratipay  | <a href="https://gratipay.com/tasdikrahman/" target="_blank"><img src="https://cdn.rawgit.com/gratipay/gratipay-badge/2.3.0/dist/gratipay.png" alt="Support via Gratipay" title="Support via Gratipay" /></a> |
| Patreon | <a href="https://www.patreon.com/tasdikrahman" target="_blank"><img src="http://i.imgur.com/ICWPFOs.png" alt="Support me on Patreon" title="Support me on Patreon" /></a> |
| £ (GBP) | <a href="https://transferwise.com/pay/d804d854-6862-4127-afdd-4687d64cbd28" target="_blank"><img src="http://i.imgur.com/ARJfowA.png" alt="Donate via TransferWise!" title="Donate via TransferWise!" /></a> |
| € Euros | <a href="https://transferwise.com/pay/64c586e3-ec99-4be8-af0b-59241f7b9b79" target="_blank"><img src="http://i.imgur.com/ARJfowA.png" alt="Donate via TransferWise!" title="Donate via TransferWise!" /></a> |
| ₹ (INR)  | <a href="https://www.instamojo.com/@tasdikrahman" target="_blank"><img src="https://www.soldermall.com/images/pic-online-payment.jpg" alt="Donate via instamojo" title="Donate via instamojo" /></a> |
