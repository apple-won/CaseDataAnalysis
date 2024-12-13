# CaseDataAnalysis
该项目是针对mazesuit软件生成的文件进一步的进行数据拆分、分组、计算绘图以及导出成表格

## 前置环境部署
### git
下载安装地址：https://git-scm.com/downloads
### pip
可参考（https://www.jianshu.com/p/2559b55a9309） 对pip进行安装


## 拉取项目,以及安装对应的依赖
使用以下命令对项目进行下载

    git clone https://github.com/apple-won/CaseDataAnalysis.git
    
下载完成后，进入下载目录下执行以下命令安装项目依赖

    pip install -r requirements.txt


## 如何使用
1、更改main.py中的 FOLDER_PATH 参数。将参数中的值更改为使用者需要数据分析文件所在的文件夹，注意末尾一定要带/

2、运行main.py，进行选择即可

2.1、半流程：将res_data中的文本数据进行进一步的分析并且生成所需要的图片，并生成结果表格

2.2、全流程：将原始数据拆分并清理不必要的数据保存在res_data中，然后执行2.1中的任务

## 新增文件夹说明
### FOLDER_PATH
需要分析的文件所在的目录，也是项目数据的根目录

数据最后导出的excle会在这个目录中
### raw_data文件夹
项目会将原本的文本进行拆分，拆分后的数据会存在这个文件夹下，会以拆分前的文件名开头进行区分
### res_data文件夹
项目会将raw_data中的文本进行清理，将文本中的异常/无效/title等信息进行清除，并对有效数据进行基本的计算，这些数据会重新保存在res_data中

### error文件夹
项目会对不需要跑/运行过程中会有问题的文件进行单独存放，放到FOLDER_PATH中的error文档中
