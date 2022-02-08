# 建木官方节点

本项目列出建木官方节点与官方认证节点

如有节点需求，也可以在本项目的 issue 中提出

若要创建自定义节点可参考[示例](https://gitee.com/jianmu-runners/jianmu-runner-example)
& [官方文档](https://docs.jianmu.dev/guide/custom-node.html)

### 如何贡献官方节点:

1. 在 [jianmu-runner-list](https://gitee.com/jianmu-runners/jianmu-runner-list/issues) 提Issue，请求贡献官方节点
2. 等待[管理员](https://gitee.com/liamjung) 回复，接受官方的仓库邀请链接
3. 在仓库中开发节点，push代码。参考[示例](https://gitee.com/jianmu-runners/jianmu-runner-example)
4. fork [jianmu-runner-list](https://gitee.com/jianmu-runners/jianmu-runner-list) 仓库， 提交pr：
    * 添加项目[release_dsl](https://gitee.com/jianmu-runners/jianmu-runner-list/tree/master/release_dsl) ，用于自动发版
    * 在[project_group.yml](https://gitee.com/jianmu-runners/jianmu-runner-list/blob/master/project_group.yml) 和 [README.md](https://gitee.com/jianmu-runners/jianmu-runner-list/blob/master/README.md) 中添加节点信息
5. 在仓库里创建`tag`，该事件触发自动发版，若需要删除已创建的tag，请联系[管理员](https://gitee.com/liamjung)
6. 发版成功，在[建木Hub](https://hub.jianmu.run/) 中查看节点

### 官方节点:

|                             Icon                             |                            Runner                            |                             Git                              |                         Release DSL                          |                            Author                            |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![img](https://img.jianmu.run/node-definition/icon/FvWtndEdOK9WmEc8WCmvKLYpy2Xv?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [docker 镜像构建](https://hub.jianmu.run/_/docker_image_build) | [jianmu-runner-docker](https://gitee.com/jianmu-runners/jianmu-runner-docker.git) | [docker_image_build.yml](./release_dsl/docker_image_build.yml) |             [邵嘉诚](https://gitee.com/MKAlieZ)              |
| ![img](https://img.jianmu.run/node-definition/icon/FpON0edVLhS5j3Kgvs9i-rwljruu?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |     [nodejs 构建](https://hub.jianmu.run/_/nodejs_build)     | [jianmu-runner-nodejs](https://gitee.com/jianmu-runners/jianmu-runner-nodejs.git) |      [nodejs_build.yml](./release_dsl/nodejs_build.yml)      |             [邵嘉诚](https://gitee.com/MKAlieZ)              |
| ![img](https://img.jianmu.run/node-definition/icon/FuR2Q_RwpR-J1vBT5vQ9nhl3cRGG?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [scp 替换文件](https://hub.jianmu.run/_/scp_resouce) <br>[ssh 执行命令](https://hub.jianmu.run/_/ssh_cmd) | [jianmu-runner-ssh](https://gitee.com/jianmu-runners/jianmu-runner-ssh.git) | [scp_resouce.yml](./release_dsl/scp_resouce.yml) <br/>[ssh_cmd.yml](./release_dsl/ssh_cmd.yml) |             [邵嘉诚](https://gitee.com/MKAlieZ)              |
| ![img](https://img.jianmu.run/node-definition/icon/Fm-mFNmB-yLjzHprqYzStHx12E0t?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |     [企业微信通知](https://hub.jianmu.run/_/qywx_notice)     | [jianmu-runner-notice](https://gitee.com/jianmu-runners/jianmu-runner-notice.git) |       [qywx_notice.yml](./release_dsl/qywx_notice.yml)       |             [邵嘉诚](https://gitee.com/MKAlieZ)              |
| ![img](https://img.jianmu.run/node-definition/icon/FikR5g_gILRZjr-olpMqypjhfuj3?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [git clone](https://hub.jianmu.run/_/git_clone) <br>[git push](https://hub.jianmu.run/_/git_push) | [jianmu-runner-git](https://gitee.com/jianmu-runners/jianmu-runner-git.git) | [git_clone.yml](./release_dsl/git_clone.yml)<br />[git_push.yml](./release_dsl/git_push.yml) |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/FuldakfWy16et8gfoLhrhqjmrFgA?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [建木 Hub 节点定义版本发布](https://hub.jianmu.run/_/hub_publish) | [jianmu-runner-hub](https://gitee.com/jianmu-runners/jianmu-runner-hub.git) |       [hub_publish.yml](./release_dsl/hub_publish.yml)       |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FjLa8W_mgaQc6ZuZ_JccCyxY4wDr?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [七牛云文件上传](https://hub.jianmu.run/_/qiniu_upload) <br> [七牛云上传 ssl 证书](https://hub.jianmu.run/_/qiniu_ssl_upload) <br> [七牛云域名 ssl 证书更新](https://hub.jianmu.run/_/qiniu_domain_ssl_update) | [jianmu-runner-qiniu](https://gitee.com/jianmu-runners/jianmu-runner-qiniu.git) |                              -                               | [老技](https://gitee.com/liamjung) <br> [comyan](https://gitee.com/comyan) <br>[冯浩](https://gitee.com/qbhfh) |
| ![img](https://img.jianmu.run/node-definition/icon/FjIcOhP7DXyU8LfuoqkQ96hK7itw?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |      [maven 构建](https://hub.jianmu.run/_/maven_build)      | [jianmu-runner-maven](https://gitee.com/jianmu-runners/jianmu-runner-maven.git) |       [maven_build.yml](./release_dsl/maven_build.yml)       |             [邵嘉诚](https://gitee.com/MKAlieZ)              |
| ![img](https://img.jianmu.run/node-definition/icon/FhaFsSZDMEklnTnzLc1qcj1IWXH5?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [飞书通知-文本](https://hub.jianmu.run/_/feishu_notice_text) <br> [飞书通知-富文本](https://hub.jianmu.run/_/feishu_notice_post) <br>[飞书通知-图片](https://hub.jianmu.run/_/feishu_notice_image) <br>[飞书通知-消息卡片](https://hub.jianmu.run/_/feishu_notice_interactive) | [jianmu-runner-feishu](https://gitee.com/jianmu-runners/jianmu-runner-feishu.git) | [feishu_notice_text.yml](./release_dsl/feishu_notice_text.yml) <br/>[feishu_notice_post.yml](./release_dsl/feishu_notice_post.yml) <br/>[feishu_notice_image.yml](./release_dsl/feishu_notice_image.yml) <br/>[feishu_notice_interactive.yml](./release_dsl/feishu_notice_interactive.yml) |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FhJotcreNFwAAio6zF-d75-zuCCf?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [acme 构建 ssl 证书-阿里云](https://hub.jianmu.run/_/acme_ssl_aliyun) | [jianmu-runner-acme-ssl](https://gitee.com/jianmu-runners/jianmu-runner-acme-ssl.git) |   [acme_sh_aliyun.yml](./release_dsl/acme_ssl_aliyun.yml)    |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/FjG9eU2DVdG-5eC9DUQ_juPkyie2?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [seafile 文件上传](https://hub.jianmu.run/_/seafile_upload) <br>[seafile 文件下载](https://hub.jianmu.run/_/seafile_download) | [jianmu-runner-seafile](https://gitee.com/jianmu-runners/jianmu-runner-seafile.git) | [seafile_upload.yml](./release_dsl/seafile_upload.yml)<br />[seafile_download.yml](./release_dsl/seafile_download.yml) |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/Fk5hx9DxszYY8DFuHeRW8TaJxPlu?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |    [tar 压缩/解压文件](https://hub.jianmu.run/_/pack_tar)    | [jianmu-runner-tar](https://gitee.com/jianmu-runners/jianmu-runner-tar.git) |          [pack_tar.yml](./release_dsl/pack_tar.yml)          |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FjyC_qHh_xVe2B3Ey4Iaw-Arfebv?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |    [zip 压缩/解压文件](https://hub.jianmu.run/_/pack_zip)    | [jianmu-runner-zip](https://gitee.com/jianmu-runners/jianmu-runner-zip.git) |          [pack_zip.yml](./release_dsl/pack_zip.yml)          |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/Fn38OYww-GzUxd6ygXGCTNo9FxtZ?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |   [allure报表生成](https://hub.jianmu.run/_/allure_report)   | [jianmu-runner-allure](https://gitee.com/jianmu-runners/jianmu-runner-allure.git) |     [allure_report.yml](./release_dsl/allure_report.yml)     |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FkC51eKE7Bln2PT96aERoJZCmkfz?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [钉钉通知-文本](https://hub.jianmu.run/_/dingtalk_notice_text) <br> [钉钉通知-链接](https://hub.jianmu.run/_/dingtalk_notice_link) <br> [钉钉通知-markdown](https://hub.jianmu.run/_/dingtalk_notice_markdown) <br> [钉钉通知-ActionCard](https://hub.jianmu.run/_/dingtalk_notice_action_card) <br> [钉钉通知-FeedCard](https://hub.jianmu.run/_/dingtalk_notice_feed_card) | [jianmu-runner-dingtalk-notice](https://gitee.com/jianmu-runners/jianmu-runner-dingtalk.git) | [dingtalk_notice_text.yml](./release_dsl/dingtalk_notice_text.yml) <br/>[dingtalk_notice_link.yml](./release_dsl/dingtalk_notice_link.yml) <br/>[dingtalk_notice_markdown.yml](./release_dsl/dingtalk_notice_markdown.yml) <br/>[dingtalk_notice_action_card.yml](./release_dsl/dingtalk_notice_action_card.yml) <br/>[dingtalk_notice_feed_card.yml](./release_dsl/dingtalk_notice_feed_card.yml) |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FkkmDW2a2RQLaivatCTK3yeC0t2k?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [mysql数据导入](https://hub.jianmu.run/_/mysql_import) <br> [mysql数据导出](https://hub.jianmu.run/_/mysql_export) | [jianmu-runner-mysql](https://gitee.com/jianmu-runners/jianmu-runner-mysql.git) | [mysql_import.yml](./release_dsl/mysql_import.yml) <br/>[mysql_export.yml](./release_dsl/mysql_export.yml) |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FjEh2QUcFpEZx1bocJfeGdmBKV4e?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |    [svn checkout](https://hub.jianmu.run/_/svn_checkout)     | [jianmu-runner-svn](https://gitee.com/jianmu-runners/jianmu-runner-svn.git) |      [svn_checkout.yml](./release_dsl/svn_checkout.yml)      |              [吴奇](https://gitee.com/ImageWQ)               |
| ![img](https://img.jianmu.run/node-definition/icon/FinkJWhh_h20FXgPjyYZTAu1qXo1?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [redis数据导入](https://hub.jianmu.run/_/redis_import) <br> [redis数据导出](https://hub.jianmu.run/_/redis_export) | [jianmu-runner-redis](https://gitee.com/jianmu-runners/jianmu-runner-redis.git) | [redis_import.yml](./release_dsl/redis_import.yml) <br/>[redis_export.yml](./release_dsl/redis_export.yml) |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FgFrUkBnhN6FVugnW2sMb_CGWaKF?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [smbclient操作共享文件夹](https://hub.jianmu.run/_/smbclient) | [jianmu-runner-smbclient](https://gitee.com/jianmu-runners/jianmu-runner-smbclient.git) |         [smbclient.yml](./release_dsl/smbclient.yml)         |              [吴奇](https://gitee.com/ImageWQ)               |
| ![img](https://img.jianmu.run/node-definition/icon/FlqdDvA4ayshPkXCIl9w2ka0Btpd?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |  [同步项目组](https://hub.jianmu.run/_/sync_project_group)   | [jianmu-runner-project-group](https://gitee.com/jianmu-runners/jianmu-runner-project-group.git) | [sync_project_group.yml](./release_dsl/sync_project_group.yml) |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FipbR3aFUOmzL5rqhaVTB1_1Pj1K?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |        [字符串工具](https://hub.jianmu.run/_/string)         | [jianmu-runner-string](https://gitee.com/jianmu-runners/jianmu-runner-string.git) |            [string.yml](./release_dsl/string.yml)            |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FtAyzPvqXDJBhgHLO--Q9CkdagLh?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [添加或更新组织成员](https://hub.jianmu.run/_/gitee/1.0.0-member-add)<br>[向gitee PR提交评论](https://hub.jianmu.run/_/gitee/1.0.0-pr-comment)<br/>[在gitee中创建webhook](https://hub.jianmu.run/_/gitee/1.0.0-webhook-create) | [jianmu-runner-gitee](https://gitee.com/jianmu-runners/jianmu-runner-gitee.git) |             [gitee.yml](./release_dsl/gitee.yml)             | [黄熙](https://gitee.com/canon_xi) <br/>[黄熙](https://gitee.com/canon_xi)<br /> [daihw](https://gitee.com/generations) |
| ![img](https://img.jianmu.run/node-definition/icon/FrluwwvH_hfx1GHO4c3qv2gcukCc?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |  [kubectl部署资源](https://hub.jianmu.run/_/kubectl_deploy)  | [jianmu-runner-k8s](https://gitee.com/jianmu-runners/jianmu-runner-k8s.git) |    [kubectl_deploy.yml](./release_dsl/kubectl_deploy.yml)    |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/FoYp6c62VmRSpCjk1Q4at4NHAPGd?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |          [发送邮件](https://hub.jianmu.run/_/email)          | [jianmu-runner-email](https://gitee.com/jianmu-runners/jianmu-runner-email.git) |             [email.yml](./release_dsl/email.yml)             |            [daihw](https://gitee.com/generations)            |
| ![img](https://img.jianmu.run/node-definition/icon/FroQcIBthodJ5NAQMnaZjxzmrU5s?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |       [计算文件md5](https://hub.jianmu.run/_/file_md5)       | [jianmu-runner-file-md5](https://gitee.com/jianmu-runners/jianmu-runner-file-md5) |          [file_md5.yml](./release_dsl/file_md5.yml)          |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/Fvo3th67o4pp_v61mBgEeEgx1FnN?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [构建开源项目个人贡献者列表](https://hub.jianmu.run/_/contributors_build) | [jianmu-runner-contributors](https://gitee.com/jianmu-runners/jianmu-runner-contributors.git) | [contributors_build.yml](./release_dsl/contributors_build.yml) |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/FvSdxG1UzMzITgl-qHelV7cNhlrF?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [构建开源项目团队贡献者列表](https://hub.jianmu.run/_/teams_build) | [jianmu-runner-teams](https://gitee.com/jianmu-runners/jianmu-runner-teams.git) |       [teams_build.yml](./release_dsl/teams_build.yml)       |              [黄熙](https://gitee.com/canon_xi)              |
| ![img](https://img.jianmu.run/node-definition/icon/Fub21RCA6F9__cLzeuw_KZiwSyfc?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) | [文本文件工具](https://hub.jianmu.run/_/text_file)           | [jianmu-runner-text-file](https://gitee.com/jianmu-runners/jianmu-runner-text-file.git) |       [text_file.yml](./release_dsl/text_file.yml)       |              [daihw](https://gitee.com/generations)              |
| ![img](https://img.jianmu.run/node-definition/icon/FjLa8W_mgaQc6ZuZ_JccCyxY4wDr?imageView2/2/w/30/h/30/interlace/1/q/100%7CroundPic/radius/!25.5p) |[七牛云文件上传](https://hub.jianmu.run/_/qiniu/1.0.0-file-upload) <br> [七牛云上传 ssl 证书](https://hub.jianmu.run/_/qiniu/1.0.0-ssl-upload) <br> [七牛云域名 ssl 证书更新](https://hub.jianmu.run/_/qiniu/1.0.0-domain-ssl-update) | [jianmu-runner-qiniu](https://gitee.com/jianmu-runners/jianmu-runner-qiniu.git) |    [qiniu.yml](./release_dsl/qiniu.yml)                  | [老技](https://gitee.com/liamjung) <br> [comyan](https://gitee.com/comyan) <br>[冯浩](https://gitee.com/qbhfh) |
