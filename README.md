# spine-runtimes
binary format support for 3.6 version spine skeleton

# what is this
in spine 3.6, there is no support for parsing binary format skeleton.  
this js just solves the issue

# how to use
#### offical runtime:
- load `spine.ex.js` after `spine-*.js` (choose from [build](https://github.com/EsotericSoftware/spine-runtimes/tree/3.8/spine-ts/build))
- `var skeletonBinary = new spine.SkeletonBinary(atlasLoader);`
- `var skeletonData = skeletonBinary.readSkeletonData(assetManager.get("assets/" + name + ".skel"));`

copied from [docs](https://github.com/EsotericSoftware/spine-runtimes/blob/3.6/spine-ts/canvas/example/index.html#L69)

#### cocos creator 2.1.3:
- replace content of `cocos2d-js-min.*.js` with content of `cocos2d-js-min.fae99.js`

`cocos2d-js-min.*.js` is located at `cocos-creator-project/build/*/` after the project is built
