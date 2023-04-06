pipeline{
//指定运行此流水线的节点
agent { node { label "dev_build"}}
OAOAOA    
 
//流水线的阶段
stages{
 
    //阶段1 获取代码
    stage("dev_CheckOut"){
        steps{
            script{
                println("获取代码")
            }
        }
    }
    stage("dev_Build"){
        steps{
            script{
                println("运行构建")
            }
        }
    }
}
post {
    always{
        script{
            println("流水线结束后，经常做的事情")
        }
    }
        
    success{
        script{
            println("流水线成功后，要做的事情")
        }
        
    }
    failure{
        script{
            println("流水线失败后，要做的事情")
        }
    }
        
    aborted{
        script{
            println("流水线取消后，要做的事情")
        }
        
    }
}
}
