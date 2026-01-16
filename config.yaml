port: 7890
socks-port: 7891
allow-lan: false
mode: rule
log-level: info

dns:
  enable: true
  ipv6: false
  enhanced-mode: fake-ip
  nameserver:
    - 223.5.5.5
    - 119.29.29.29

proxies:
  - name: CN-STATIC
    type: ss
    server: 119.91.5.158
    port: 8399
    cipher: aes-256-gcm
    password: cn123456

proxy-groups:
  - name: BROWSER
    type: select
    proxies:
      - CN-STATIC
      - DIRECT

rules:
  - MATCH,BROWSER
