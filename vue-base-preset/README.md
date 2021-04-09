# @vue/cli preset

## 全局安装 @vue/cli

```shell
yarn global add @vue/cli
```

## 创建项目

### 从 GitHub 获取预设
```shell
# 从 GitHub repo 使用 preset
vue create --preset vocjs/vue-base-preset project-name
```

### 将预设保存到本地

```shell
# ./my-preset 应当是一个包含 preset.json 的文件夹
vue create --preset ./my-preset project-name

# 或者，直接使用当前工作目录下的 json 文件：
vue create --preset preset.json project-name
```

### 预设保存到 @vue/cli 配置文件 .vuerc

1. 将预设保存到文件 presets 节点，键名为预设名称，值为预设对象（.vuerc 是保存在用户的 home 目录下一个 json 文件）
2. 直接使用 vue create 创建项目，并选择预设

```shell
vue create project-name
```