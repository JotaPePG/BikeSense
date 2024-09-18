### **Desinstalar o docker completamente de qualquer máquina**

`sudo systemctl stop docker` <!--(Antes de desinstalar, pare o serviço do Docker, se estiver em execução.)-->

`sudo apt-get purge docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin` <!--(Remover pacotes Docker: Desinstale o Docker, Docker CLI e outros pacotes relacionados (caso existam) com o seguinte comando:)-->

sudo apt-get autoremove -y ( Para limpar pacotes órfãos ou dependências não usadas após a remoção, execute:)

---

### **Baixar o docker version 26.0.2 pelo script oferecido pelo rancher**

`curl https://releases.rancher.com/install-docker/26.0.2.sh | sh` <!--(Isso vai baixar e executar o script de instalação fornecido pelo Rancher, que instala o Docker com a versão especificada.)-->

`sudo usermod -aG docker ubuntu`

---
