# 管理项目

项目提供了一个企业中多个组织或者部门独立使用和管理 MQTT 集群的能力，可以分配不同的角色对平台的各项能力进行更加精细化的管理。基于项目，每个组织或者部门可以单独管理自己的 MQTT 集群，并可以独立核算。在多项目的机制下，部署需建立在项目下面，并且一个部署只能属于一个项目。

## 项目列表

点击顶部菜单栏中的**部署管理**进入页面，在页面左侧可以看到项目列表。

![default_project](./_assets/default_project.png)

## 创建项目

点击**新建项目**，在弹框中输入项目名称和备注，可以创建一个新项目。

![create_project](./_assets/create_project.png)

## 在项目下创建部署

选中左侧项目，可以在选中项目下创建部署。

![create_deployment_under_project](./_assets/create_deployment_under_project.png)

## 移动部署到其他项目

1. 点击部署右上角的菜单，选择**移动到**。

![move_project_menu](./_assets/move_project_menu.png)

2. 在**选择项目**下拉列表中选择目标项目。

![move_project](./_assets/move_project.png)

3. 点击**确认**后，便可以将部署移动到目标项目下。


## 更新项目

选择一个项目，点击右上角修改按钮，可以对项目名称和描述进行修改更新。

![update_project_menu](./_assets/update_project_menu.png)


## 删除项目

> 删除项目之前请确保项目下没有部署。

选择一个项目，点击右上角删除按钮。

![delete_project](./_assets/delete_project.png)

## 关联子用户账号

选择一个项目，点击右上角关联账号按钮，可设置该项目[子用户](./user.md)。

![delete_project](./_assets/link_subuser.png)
