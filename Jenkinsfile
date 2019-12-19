node {  
    stage('Build') { 
        echo 'test ${params.ELASTIC_TARGET}'
        sh 'curl -XPUT http://elastic:9200/newindex'
        sh 'curl -XPUT http://elastic:9200/newindex/_mapping/newmapping -d \'{ "newmapping": { "properties": { "id": { "type": "string" }, "actif": { "type": "boolean" }}}}\''
    }
}
