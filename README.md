# Firewall UFW

## 1 - Instalação
```
sudo apt-get install ufw
```

## 2 - Definindo políticas padrão
```
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## 3 - Permitindo conexão via SSH
```
sudo ufw allow ssh
```
ou 
```
sudo ufw allow 22
```

## 4 - Habilitando o firewall
```
sudo ufw enable
```

## 5 - Definindo faixa e protocolo
```
sudo ufw allow 6000:6007/tcp
```

## 6 - Endereço específico
```
sudo ufw allow from 222.105.0.6
```

## 7 - Sub-redes
```
sudo ufw allow from 203.0.113.0/24
```

## 8 - Interface de rede
```
sudo ufw allow in on eth0
```

## 9 - Negar conexões
```
sudo ufw deny http
```

## 10 - Listar regras
```
sudo ufw status numbered
```

## 11 - Deletando regra
```
sudo ufw delete 2
```

## 12 - Disabilitando firewall
```
sudo ufw disable
```

## 13 - Apagar todas regras
```
sudo ufw reset
```
