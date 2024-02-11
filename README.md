# YouTube ReVanced Extended Magisk Module

Get the [latest CI release](https://github.com/MANCrimSon/YouTube-ReVanced-Extended/releases).

Use [**zygisk-detach**](https://github.com/j-hc/zygisk-detach) to detach YouTube from Google Play. 

<details><summary><big>Features</big></summary>
<ul>
 <li> <a href="https://github.com/YT-Advanced/ReX-patches">Patches</a> </li>
 <li> Can build Magisk modules and non-root APKs</li>
 <li> Updated daily with the latest versions of apps and patches</li>
 <li> Optimize APKs and modules for size</li>
 <li> Modules</li>
    <ul>
     <li> recompile invalidated odex for faster usage</li>
     <li> receive updates from Magisk app</li>
     <li> do not break safetynet or trigger root detections</li>
     <li> handle installation of the correct version of the stock app and all that</li>
     <li> support Magisk and KernelSU</li>
    </ul>
</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in ReVanced patches. You may want to disable it.
</details>

## To include/exclude patches or patch other apps
[**See the list of patches**](https://j-hc.github.io/rvmm-config-gen/)

 * Star the repo :eyes:
 * Use the repo as a [template](https://github.com/new?template_name=revanced-magisk-module&template_owner=j-hc)
 * Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

also see here [`CONFIG.md`](./CONFIG.md)

## Building Locally
### On Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/MANCrimSon/YouTube-ReVanced-Extended/main/build-termux.sh)
```

### On Desktop
```console
$ git clone https://github.com/MANCrimSon/YouTube-ReVanced-Extended
$ cd YouTube-ReVanced-Extended
$ ./build.sh
```
