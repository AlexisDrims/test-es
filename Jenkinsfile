node {  
    stage('Build') { 
        sh "echo '${params.ELASTIC_TARGET}'"
        sh "echo '${env.ELASTIC_TARGET}'"
        sh "echo '${ELASTIC_TARGET}'"
        echo 'test params.ELASTIC_TARGET = ${params.ELASTIC_TARGET}'
        echo 'test env.ELASTIC_TARGET = ${env.ELASTIC_TARGET}'
        echo 'test ELASTIC_TARGET = ${ELASTIC_TARGET}'
        sh 'curl -XPUT http://elastic:9200/newindex'
        sh 'curl -XPUT http://elastic:9200/newindex/_mapping/newmapping -d \'{ "newmapping": { "properties": { "id": { "type": "string" }, "actif": { "type": "boolean" }}}}\''
    }
}
