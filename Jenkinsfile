// 流水线脚本

pipeline{
    // 任何代理可用就可以执行
    agent any
    environment{
    hello="hello jenkins"
    }
    stages{
        // 流水线的所有阶段
        // 1、编译
        stage('代码编译'){
        agent{
            docker 'maven:3-alpine'
            }
            steps{
                echo "代码编译"
                echo "代码编译111"
                echo "${hello}"
            }

        }

        // 2、测试
        stage('代码测试'){
            steps{
                echo "代码测试"
            }
        }
        // 3、打包
        stage('打包'){
            steps{
                echo "打包"
            }
        }

        // 4、部署
        stage('部署'){
            steps{
                echo "部署"
            }
        }
	}
}

