# ELK-Stack

## Logstash

初始配置文件 with elasticsearch option

input {
	stdin {}
}


output {
	stdout {
		codec => rubydebug
	}
    elasticsearch { 
		hosts => ["10.67.180.30:9200"]
		}
}
