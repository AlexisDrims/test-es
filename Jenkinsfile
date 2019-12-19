node {  
    stage('Build') { 
        sh 'curl -XPUT http://elastic:9200/newindex'
        sh 'curl -XPUT http://elastic:9200/newindex/_mapping/newmapping -d \'{ "newmapping": { "properties": { "id": { "type": "string" }, "actif": { "type": "boolean" }}}}\''
    }
}
