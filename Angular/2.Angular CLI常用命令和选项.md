# Angular CLI常用命令和选项

## 1.初始化命令和选项
初始化命令格式为：
```js
ng new <name> [options]
```
可以简写为：
```js
ng n <name> [options]
```
- name 是创建项目的名称
- options 附加参数

### 1.1 options 常用参数
- --routing=false|true 是否需要创建路由
- --style=css|scss|sass|less|styl 选择添加的样式文件格式
- --inlineTemplate=true|false （简写：--inline-template或-t) 是否使用内联模板生成组件，组件模板标记将在组件内生成，而不是在单独的文件中生成
- --inlineStyle=true|false (简写：--inline-style或-s）是否生成具有内联样式的组件，组件样式将在组件内生成，而不是在单独的文件中生成
- --skipTests=true|false （简写：-S) 如果为true,则不会为新项目生成spec.ts测试文件
- --minimal=true|false 如果为true,则相当于--inlineTemplate=true --inlineStyle=true --skipTests=true 以及不含e2e测试文件
- --interactive=true|false 如果为false，则禁用交互式输入提示，相当于--routing=false --styl=css
- --defaults=true|false 如果为true，同--interactive=true
以上参数默认值全部为false.

## 2.创建命令和选项
创建命令的格式为：
```js
ng generate <type> [options]
```
可以简写为：
```js
ng g <type> [options]
```

### 2.1 常用的type
- 创建组件 ng g component new-component
    - 选项如下：
    - --inlineStyle=true|false 默认为false，如果为true生成具有内联样式的组件
    - --inlineTemplate=true|false 默认为false，如果为true生成内联模板
    - --skipTests=true|false 默认为false，如果为true不为组件创建spec.ts测试文件
    - --flat=true|false 默认为false，如果为true则在当前项目的根目录下创建新文件
- 创建指令 ng g directive new-directive
- 创建管道 ng g pipe new-pipe
- 创建服务类 ng g service new-service
- 创建类 ng g class new-class
- 创建接口 ng g interface new-interface
- 创建枚举类 ng g enum new-enum
- 创建模块 ng g module new-module
