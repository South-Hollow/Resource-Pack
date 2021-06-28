# SouthHollow Network Resource Pack
The resource pack that gets applied to all players when they join the SouthHollow network.

![GitHub release (latest by date)](https://img.shields.io/github/v/release/South-Hollow/Resource-Pack?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/South-Hollow/Resource-Pack?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/South-Hollow/Resource-Pack?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/South-Hollow/Resource-Pack?style=flat-square)


## Releases
All releases can be found in the [releases page](https://github.com/South-Hollow/Resource-Pack/releases), along with a specfic changelog. The zip file attachment will be for the currently most-supported version at that time. For simplicity sake, please access the branch of the pack version you'd like to see instead of trying to download it off the releases page.

## Currently Supporting:
- Minecraft 1.16.5
- Minecraft 1.17.x

## How To (Server Admins)
We currently use [Phoenix616's ResourcepacksPlugins](https://github.com/Phoenix616/ResourcepacksPlugins) to send the pack to player clients and keep track of them so it's not unnessesarily re-sent. It is running on our proxy of choice, [Velocity](https://github.com/VelocityPowered/Velocity). There is a `config.yml` file which is used to update information about the packs. However, it is unlikely that you'll be editing it. Here's why:

The `config.yml` file is setup to point the pack download to this Github repository. This means that GitHub acts as our CDN, and any that the pack can be updated without having to edit the following config.
```
packs:
  globalpack:
    restricted: false
    permission: [ REDACTED ]
    variants:
    - url: https://github.com/South-Hollow/Resource-Pack/raw/ver/1.16.5/SouthHollow.zip
      hash: [ REDACTED ]
      version: '1.16'
      restricted: false
      permission: [ REDACTED ]
    - url: https://github.com/South-Hollow/Resource-Pack/raw/ver/1.17/SouthHollow.zip
      hash: [ REDACTED ]
      version: '1.17'
      restricted: false
      permission: [ REDACTED ]
```
Typically, the proxy will need to be rebooted in order for all the changes to be made correctly. While the `/vrp reload` command exists, limited success has been had with it, and using it is discouraged.

## How To (Pack Contributors)
See [Contributing](https://github.com/South-Hollow/Resource-Pack/blob/main/CONTRIBUTING.md)

## Terms of Use
See [Terms](https://github.com/South-Hollow/Resource-Pack/blob/main/TERMS.txt)


## Important Links
* [Official Website](https://southhollow.net/)
* [Discuss](https://github.com/South-Hollow/Resource-Pack/discussions)
* [Issues](https://github.com/South-Hollow/Resource-Pack/issues)
* [Projects](https://github.com/South-Hollow/Resource-Pack/projects)
* [Contact Us](mailto:southhollowmc@gmail.com)
