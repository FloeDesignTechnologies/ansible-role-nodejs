Ansible Node.js Role
=========

[![Build Status](https://secure.travis-ci.org/martinmicunda/ansible-role-nodejs.png)](http://travis-ci.org/martinmicunda/ansible-role-nodejs) [![Ansible Galaxy](http://img.shields.io/badge/galaxy-mm.nodejs-blue.svg)](https://galaxy.ansible.com/list#/roles/1581) [![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg)](#)

An ansible role for installing Node.js and NPM.

Requirements
------------

#### Ansible

It has been tested on Ansible 1.7 and above.

#### Platforms

Currently it's been developed for, and tested on Ubuntu.

Role Variables
--------------

List of default variables available in the inventory:

| Name                    | Default   | Description      |
| ----------------------- | --------- | ---------------- |
| nodejs_version          | latest    | Node.js version  |
| apt_cache_valid_time    | 3600      | Cache valid time |

Example Playbook
----------------

Add `mm.nodejs` to your roles and overwrite default vars (optional) in your playbook file.

    - hosts: all
      roles:
         - role: mm.nodejs
      vars:
         - nodejs_version: "0.10.31"  

License
-------

    The MIT License
    
    Copyright (c) 2014 Martin Micunda  

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
