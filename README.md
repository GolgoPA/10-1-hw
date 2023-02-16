# 10-1-hw# Домашнее задание к занятию 10.1 «Keepalived/vrrp»

---

### Задание 1

Разверните топологию из лекции и выполните установку и настройку сервиса Keepalived. 

```
vrrp_instance test {

state "name_mode"

interface "name_interface"

virtual_router_id "number id"

priority "number priority"

advert_int "number advert"

authentication {

auth_type "auth type"

auth_pass "password"

}

unicast_peer {

"ip address host"

}

virtual_ipaddress {

"ip address host" dev "interface" label "interface":vip

}

}

```

*Пришлите скриншот рабочей конфигурации и состояния сервиса для каждого нода.
![10-1-1](./hw-10-1/10-1-1.png)
![10-1-2](./hw-10-1/10-1-2.png)
![10-1-3](./hw-10-1/10-1-3.png)
![10-1-4](./hw-10-1/10-1-4.png)
