sa-chef-sdk
===========

[![Build Status](https://travis-ci.org/softasap/sa-chef-sdk.svg?branch=master)](https://travis-ci.org/softasap/sa-chef-sdk)

What's Included?
The Chef Development Kit contains everything you need to start using Chef, along with the tools essential to managing the code that runs your business.

ChefDK contains:

An early version of a brand new command-line tool, chef, that aims to streamline Chef workflow, starting with new generators.
The well-known cookbook dependency manager Berkshelf.
The Test Kitchen integration testing framework.
ChefSpec, which makes unit testing cookbooks a breeze.
Foodcritic, a linting tool for doing static code analysis on cookbooks.
All of the Chef tools you're already familiar with: Chef Client, Knife, Ohai and Chef Zero.


Tests cover LTS releases only

Example of usage (all parameters are optional)

Simple

  roles:
    - {
        role: "sa-chef-sdk"
      }


Advanced:


  roles:
    - {
        role: "sa-chef-sdk",
        chef_sdk_version: "0.14.25",
        option_install_ruby: true,
        option_ruby_install_setsystem: true,
        option_install_git: true,

      # ruby dependency
        rubies_location: /opt/rubies,
        chruby_version: 0.3.9,
        ruby_install_version: 0.6.0,
        ruby_install_setsystem: true,
        ruby_version: 2.1.9        
      }
