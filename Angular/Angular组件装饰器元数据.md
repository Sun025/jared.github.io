# Angular组件装饰器元数据
元数据告诉Angular到哪里获取它需要的主要信息，以创建和展示这个组件类及其视图。Angular会根据元数据的值来渲染组件并执行组件的逻辑。

元数据的配置选项：
- selector 是一个CSS选择器，它会告诉Angular，一旦在模板HTML中找到了这个选择器对应的标签，就创建并插入App组件的一个实例的视图。
- templateUrl 组件的HTML模板文件，这个模板文件定义了组件的视图
- styleUrl 组件的样式文件
- animations 当前组件的动画列表
- changeDetection 指定使用的变化监测策略
- encapsulation 当前组件使用的样式封装策略
- entryComponents 一组应该和当前组件一起编译的组件
- exportAs 给指令分配一个变量，使其可以在模板中使用
- inputs 指定组件的输入属性
- interpolation 当前组件模板中使用的自定义插值标记，默认是{{}}
- moduleld 包含该组件模板的ID，被用于解析模板和样式的相对路径
- outputs 指定组件的输出属性，显示其他组件可以订阅的输出事件的类属性名称列表
- providers 指定该组件及其所有子组件可用的服务依赖注入
- queries 设置需要被注入组件的查询
- viewProviders 指定该组件及其所有子组件可用的服务