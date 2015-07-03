pillow-prerequisites
====================


Requirements
------------

Tested with Pillow 2.9.0 on:

* Ubuntu 12.04 Precise Pangolin
* Ubuntu 14.04 Trusty Tahr


Role Variables
--------------

You can enable Pillow's features by set up the following vars:

    pillow_tkinter: yes
    pillow_jpeg: yes
    pillow_openjpeg: yes
    pillow_png: yes
    pillow_tiff: yes
    pillow_freetype2: yes
    pillow_littlecms2: yes
    pillow_webp: yes


Example Playbook
----------------

Example:

    - hosts: servers
      roles:
        - { role: korzeniewskipl.pillow-prerequisites, pillow_tkinter: no }
