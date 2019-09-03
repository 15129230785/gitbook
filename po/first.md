
## 怎么合代码

:point_right: 这是视频[**https://onebox.huawei.com/v/ca397a7dbd88790893dd7e79ffe5e4c5**](https://onebox.huawei.com/v/ca397a7dbd88790893dd7e79ffe5e4c5)


![img](/img/mr-process.png)


>   下面以软件管理服务为例[https://code.huawei.com/iManager_U2000-M_V3/SWMWebsite](https://code.huawei.com/iManager_U2000-M_V3/SWMWebsite)

### 步骤1 克隆代码到本地
```
# git clone git@code-xa.huawei.com:iManager_U2000-M_V3/SWMWebsite.git
# cd SWMWebsite
# git checkout MAEV100R020C10
```

### 步骤2 基于主干拉个人开发分支
```
# git checkout -b MAEV100R020C10_工号

```

### 步骤3 开发代码，提交到本地，推送到远程仓库
```
# git push origin MAEV100R020C10_工号

```

### 步骤4 在git网站上提MR
![img](/img/MR.png)

### 步骤5 Committer合入
> [!WARNING|style:flat]
> MAEV100R020C10自动合V_MAEV100R020C10有时会失效，项目经理每次出版本前一定要对比两个分支无差异。



&nbsp;

<br>


