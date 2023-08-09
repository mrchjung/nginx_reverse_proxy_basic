# nginx_reverse_proxy_basic

basic form of reverse proxy using nginx, on Docker

load balancing option

# 참조 : http://nginx.org/en/docs/stream/ngx_stream_upstream_module.html

ip_hash - ip로 분배한다. 만약 A라는 ip가 server1에 접속했으면 이후에도 server1에 계속 접속하게 되며, 한번 접속한 ip는 계속 같은 서버를 사용한다.

least_conn - 가중치를 고려하면서 연결된 접속자가 가장 적은 서버로 분배

least_time - 연결된 접속자가 가장 적으면서 + 평균 응답시간이 가장 적은 쪽으로 분배
