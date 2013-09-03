# Mac Tapas

note: veewee current only supports osx installations through VMWare
Fusion. Virtualbox support [is in development]. Until then, both a [VMWare
Fusion] installation ($50) and the [Vagrant vmware] plugin ($80) are
required.

[is in development]: https://github.com/jedi4ever/veewee/pull/770
[VMWare Fusion]: https://www.vmware.com/products/fusion
[Vagrant vmware]: http://www.vagrantup.com/vmware

* [Download "OSX Moutain Lion"] from the Mac App Store
* Install VMWare Fusion
* [Install Vagrant](http://downloads.vagrantup.com/)

[Download "OSX Moutain Lion"]: https://itunes.apple.com/en/app/os-x-mountain-lion/id537386512?mt=12

After installing all the required tools, clone this repository and install
the required gems:

    $ git clone https://github.com/JeanMertz/mac-tapas.git
    $ cd mac-tapas
    $ bundle install --binstubs

Next, define and build the osx template.

    $ bin/veewee fusion define osx-box osx
    $ bin/veewee fusion build osx-vbox`

You can now ssh into the new machine using `ssh vagrant@ip.addr.ess`.
