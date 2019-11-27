## 1.FYMaven
组件打包发布到maven仓库
 

## 2.使用
### a.在组件工程build.gradle中添加如下

apply from: 'https://raw.githubusercontent.com/fydevils/FYMaven/master/mvn_sync.gradle'

### b.参数配置两种方式
#### 1)gradle.properties文件中添加
'''
ARTIFACT_ID = t_test
GROUP_ID=com.foryou.common
'''

#### 2)在组件build.gradle最底部添加
'''
mavenConfig{
    artifactId = "t_test"
    groupId = "com.foryou.common"
}
'''

### c.使用uploadArchives命令进行上传
'''
eg:

gradlew t_test:uploadArchives -P USERNAME=*** -P PASSWORD=*** -P BUILD_VERSION=***

'''



