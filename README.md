## 1.FYMaven
������������maven�ֿ�
 

## 2.ʹ��
### a.���������build.gradle���������

apply from: 'https://raw.githubusercontent.com/fydevils/FYMaven/master/mvn_sync.gradle'

### b.�����������ַ�ʽ
#### 1)gradle.properties�ļ������
'''
ARTIFACT_ID = t_test
GROUP_ID=com.foryou.common
'''

#### 2)�����build.gradle��ײ����
'''
mavenConfig{
    artifactId = "t_test"
    groupId = "com.foryou.common"
}
'''

### c.ʹ��uploadArchives��������ϴ�
'''
eg:

gradlew t_test:uploadArchives -P USERNAME=*** -P PASSWORD=*** -P BUILD_VERSION=***

'''



