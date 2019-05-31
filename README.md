# 基于cocos creator的UI框架
中心思想, 将所有的UI窗体分为3类管理normal(普通窗体), fixed(固定窗体), popup(弹出窗体), 不同类型的窗体放置在不同的节点上, 统一管理

## 项目介绍
        -- UIManager ***
        UI窗体管理类, 控制的所有窗体的加载, 显示和释放
        -- BaseUIForm **
        UI窗体的基类, 所有的窗体应当继承它, 并重写init方法
        -- UIMaskManager **
        UI窗体的遮罩管理类, 为UI窗体添加一个背景阴影
        -- UIMaskScript *
        设置遮罩样式和取消遮罩
        -- UIType *
        设置窗体类型, 在BaseUIForm中设置其属性
        -- UILoader *
        用于加载UI窗体

        -- ConfigUIFrame *
        配置UI窗体 名称与路径的对应关系
        -- SysDefine *
        设置一些定义的路径和对应结点名称


## 使用方法
        下载: 进入script文件夹中, 将UIFrame文件夹拷贝到你自己的项目中

        场景结点设置, 如果UIRoot及子节点设置的和我不同, 请到SysDefind中修改
![](https://github.com/kirikayakazuto/UIFrameWorld/blob/master/UIROOT_dist.png)

        1, 新建一个UI窗体, 并为它创建一个脚本, 脚本继承自BaseUIForm, 重写属性CurrentUIType设置为窗体对应属性
        2, 重写init方法, 并获取参数obj, 对UI窗体进行数据初始化
        3, 更多使用方法请看test








