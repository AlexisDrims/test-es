node {  
    stage('Build') { 
        sh "echo build on '${ELASTIC_TARGET}'"
        sh 'curl -XPUT http://${ELASTIC_TARGET}/newindex'
        sh 'curl -XPUT http://${ELASTIC_TARGET}/newindex/_mapping/newmapping -d \'{ "newmapping": { "properties": { "id": { "type": "string" }, "actif": { "type": "boolean" }}}}\''
    }
}
