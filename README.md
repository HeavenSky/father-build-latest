# father-build

See our [main repo](https://github.com/umijs/father) for more information.

## 重点声明
* 本项目是完全fork自father-build
* 对应版本查看`package.json`的`keywords`属性
* 因为原项目有bug,且是死锁版本的,本项目改为不锁死版本。

## 相对改动
* 本项目仅仅是将father-build依赖做了版本升级
* 将`rollup-plugin-commonjs`替换成`@rollup/plugin-commonjs`
* 将`babel-preset-mbp`已经依赖的做了移除

## 使用方法
其实配置均参考 father-build 和 rollup
```sh
npminstall -c father-build-mbptest
npx father-build
```

## 替换方法
```sh
sed -i '' 's+rollup-plugin-commonjs+@rollup/plugin-commonjs+' lib/getRollup* src/getRollup*
```