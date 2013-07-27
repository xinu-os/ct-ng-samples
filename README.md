ct-ng-samples
=============

Sample files for building crosstool-NG cross-compilers for the Xinu
platform

HOW-TO
------

Install [crosstool-NG][ct-ng] on your system.

Clone this repository and change into the directory of the clone.

If you want to see all available samples, `ct-ng list-samples` will list
all global and local samples. If you are in this repository's directory you
should see some samples with the [L] prefix (meaning they are local). These
local samples are the samples used to build the Xinu kernel.

Depending on the kernel platform you are targeting, select the appropriate
sample and start the build process:

    ct-ng x86_64-unknown-elf
    ct-ng build

If all goes well you should have a cross-compiler for the selected
platform. If you want to change the destination or other cross-compiler
parameters you can run `ct-ng menuconfig`.

License
-------

[crosstool-NG][ct-ng] is (mostly) licensed under the GNU General Public
License version 2. Since this repository contains configuration files for
building the cross-compiler, they are also licensed under GPLv2. The full
text of GPLv2 is found in the LICENSE file.


[ct-ng]: http://crosstool-ng.org/
