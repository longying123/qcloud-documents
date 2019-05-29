## 功能说明
COSBrowser 工具即 COS 客户端工具，用户可以通过可视化界面方便的进行数据的上传、下载和管理。

>!
>
>- COS Browser PC端（Windows/macOS）会使用系统配置的代理来尝试网络连接，请确保您的代理配置正常或请停用无法连接互联网的代理配置。Windows 用户可在操作系统的【Internet 选项】中查询，macOS 用户可在【网络偏好设置】中查询。
- 使用该工具上传同名文件，会覆盖较旧的同名文件，不支持校对是否存在同名文件的功能。

## 下载安装
### 下载并安装
|支持平台|下载地址|
|:---|:---|
|Windows PC端|[Windows ](https://cos5.cloud.tencent.com/cosbrowser/releases/cosbrowser-setup-latest.exe)|
|macOS PC端|[macOS ](https://cos5.cloud.tencent.com/cosbrowser/releases/cosbrowser-latest.dmg)|
|Android 移动端|[Android ](http://)|
|iOS 移动端|[iOS ](http://)|

### 登录
打开下载好的COSBrowser进入登录页面
- PC端（Windows/macOS）
![](https://main.qcloudimg.com/raw/d4159f52bbf13f3d726376fd73dcfffc.png)
  - 云 API 密钥 SecretId/SecretKey : 用户可使用云 API 密钥 SecretId 和 SecretKey（不支持项目密钥）进行登录，该密钥可从 COS 控制台左侧栏【密钥管理】或 [云 API 密钥控制台](https://console.cloud.tencent.com/cam/capi) 获取，成功登录后密钥会保存在**历史密钥**中。
  - 历史密钥：单击**历史密钥**，可查看并使用已在该电脑成功登录过的云 API 密钥。

- 移动端（Android/iOS）
COSBrowser 移动端支持以下两种登录方式：
  - 微信快捷登录：通过微信创建的腾讯云账号，可以使用微信快捷登录方式快速登录 COSBrowser 。
  - 永久密钥登录：用户可使用云 API 密钥 SecretId 和 SecretKey（不支持项目密钥）进行登录，该密钥可从 COS 控制台左侧栏【密钥管理】或 [云 API 密钥控制台](https://console.cloud.tencent.com/cam/capi) 获取，登录后会永久保持该账号的登录状态。
>!
>目前暂不支持使用 QQ 快捷登录，若用户的腾讯云账号为 QQ 账号所创建的，请使用云 API 密钥方式登录。

## 使用方法
- 管理文件/文件夹
  - 创建文件夹
    - 在 COSBrowser 首页单击选择存储桶；
    - 单击**新建文件夹**；
    - 填写文件夹名并确认。
    >说明：
    >文件夹名称长度限制在255个字符内，可用数字、英文的组合；
    >文件夹名称不可包含 \ / : * ? " | < > 等特殊字符;
    >不允许以 .. 作为文件夹名称。

  - 上传文件/文件夹
在指定的存储桶或目录内，单击**上传文件或上传文件夹**，选择要上传的文件或文件夹，即可完成文件或文件夹的上传。
  >!
  >COSBrowser 移动端(Android/iOS)仅支持上传图片

  - 下载文件/文件夹
    - 在指定的存储桶或目录内，选中要下载的文件/文件夹；
    - 单击**下载**，即可以默认下载方式进行下载；
    - 用户还可以选择**高级下载**，进行下载的方式配置。
![](https://main.qcloudimg.com/raw/9343e8f1dea5e91370853fea24fd4ead.png)
    >!
    >- COSBrowser 移动端(Android/iOS)没有**高级下载**模式，不支持下载文件夹；
    >- COSBrowser 移动端(Android/iOS)仅支持下载图片格式文件。

  - 复制、粘贴文件/文件夹
    - 在指定的存储桶或目录内，选中要复制的文件/文件夹，单击**复制**；
    - 进入要粘贴文件的存储桶或目录内，单击**粘贴**。
    >!
    >- 公有云地域和金融云地域之间不知道相互复制、粘贴；
    >- 若复制文件的源地址和目的地址一致，会默认对同名文件进行重命名，若复制文件的源地址和目的地址不一致，则会覆盖同名文件；
    >- COSBrowser 移动端(Android/iOS)不支持复制、粘贴文件夹。

  - 重命名文件/文件夹
    - 在指定的存储桶或目录内，选中要重命名的文件/文件夹，单击**重命名**；
    - 输入新的文件名称。
    >!
    >文件夹无法进行重命名操作。

  - 删除文件/文件夹
  在指定的存储桶或目录内，选中要删除的文件/文件夹，单击**删除**。
  >说明：
  >删除操作可选中多个文件/文件夹批量进行。

- 更多操作
  - 通用设置
单击**设置**，进入 COSBrowser 的设置界面修改通用配置，如语言、服务端域名、是否使用HTTPS等。
  - 上传/下载参数配置
    - 文件并发数：设置文件上传/下载的并发任务数，超过最大并发数量的任务会进入等待队列，待前序任务完成后执行；
    - 分片并发数：设置文件上传/下载的分片数量；
    - 失败重试次数：设置文件上传/下载的重试失败次数。
## 更新日志

更新日志：
- PC端（Windows/macOS）:  [change log](https://github.com/tencentyun/cosbrowser/blob/master/changelog.md)
- 移动端（Android/iOS）:  [待建立](https://github.com/tencentyun/cosbrowser/blob/master/changelog.md)
## 反馈和建议

欢迎提交反馈和建议：[cosbrowser issues](https://github.com/tencentyun/cosbrowser/issues)

