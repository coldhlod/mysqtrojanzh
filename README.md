## Trojan-Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/coldhlod/mysqtrojanzh)

������������Ϊ��վ���������443�˿ڼ���...

## ʳ�÷���

����һ��v2rayN�ͻ��˵ı���config.json�ļ����޸�����Ĳ��ִ��벢ճ��������JSON�ļ��Ķ�Ӧ�����У������Զ���ڵ㼴��...

  "outbounds": [
    {
      "tag": "proxy",
      "protocol": "trojan",
      "settings": {
        "servers": [
          {
            "address": "��ѡIP",
            "method": "chacha20",
            "ota": false,
            "password": "����",
            "port": 443,
            "level": 1
          }
        ]
      },
      "streamSettings": {
        "network": "ws",
        "security": "tls",
        "tlsSettings": {
          "allowInsecure": false,
          "serverName": "������ַ.dev"
        },
        "wsSettings": {
          "path": "/",
          "headers": {
            "Host": "������ַ.dev"
          }
        }
      },
      "mux": {
        "enabled": false,
        "concurrency": -1
      }
    },

��ע�ⲻ�ɿ���MUX��

## ����

����bclswl0827���е���Ŀ�޸�

ԭ��������https://github.com/bclswl0827/v2ray-heroku
