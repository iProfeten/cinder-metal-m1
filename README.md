<p align="center">
  <img src="https://libcinder.org/docs/_assets/images/cinder_logo.svg" alt="Cinder Logo" width="256" height="auto"/>
</p>


This version of cinder builds on Apple M1 and also includes the Cinder Metal Block under blocks.

Please note that Cinder depends on a few submodules. The simplest way to clone it is:<br />
```
git clone --recursive
https://github.com/iProfeten/cinder-metal-m1.git

Easy start:
1. Clone repo
2. create a build dir parallell to source
3. cd build dir
3. cmake ../src -DCMAKE_OSX_ARCHITECTURES="arm64" 
4. then run cmake --build .
5. Use tinderbox from the tools as usual to generate project. Metal should be found there now.
6. Make sure you add ARC (under build options/Apple clang -language -Objective-C/Objective-c Automatic Reference Counting) if compiling with metal as well as the metal framework and the quartz framework (for core animation)

Cinder is released under the [Modified BSD License](COPYING). Please visit [our website](https://libcinder.org) for more information.

Also be sure to check out the [User Forum](http://discourse.libcinder.org).
