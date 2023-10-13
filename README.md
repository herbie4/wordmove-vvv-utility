# wordmove vvv utility (outdated)
 Wordmove utility for VVV
 
 ~~Better to use this option: https://github.com/welaika/vvv-wordmove~~
 But nowadays it is already included in VVV.
 
 -----
 # OUTDATED

 This utility will set up [Wordmove](https://github.com/welaika/wordmove/) on your [VVV](https://github.com/Varying-Vagrant-Vagrants/VVV).
 It will install WordMove version 4.0.1.
 
 ## Usage

In your `custom.yml` file add under `utilities`:

```yml
utilities:
  core:
    - php72
  wordmove:
    - wordmove
utility-sources:
  wordmove:
    repo: https://github.com/herbie4/wordmove-vvv-utility.git
    branch: master
```

The `core` utilities are there by default, and `wordmove` doesn't depend on them.

Once you add it, be sure you re-provision your VVV with `vagrant reload --provision`.
