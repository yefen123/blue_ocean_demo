pipeline {
	//运行在任意的可用节点上
	agent any
	stages {
		stage('阶段名称：master_拉取代码') {
			steps("步骤名称：拉取代码change"){ 
				echo '打印：拉取代码' 
			}
		}
		stage('阶段名称：master_编译构建') {
			steps { 
				echo '打印：编译构建' 
			}
		}
		stage('阶段名称：master_项目部署') {
			steps { 
				echo '打印：项目部署' 
			}
		}
	}
    post{
        always{
            echo "阶段完成后动作"
        }
    }
}
