### **Desinstalar o docker completamente de qualquer máquina**

```bash
sudo systemctl stop docker
```

 <!--(Antes de desinstalar, pare o serviço do Docker, se estiver em execução.)-->

```bash
sudo apt-get purge docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

 <!--(Remover pacotes Docker: Desinstale o Docker, Docker CLI e outros pacotes relacionados (caso existam) com o seguinte comando:)-->

sudo apt-get autoremove -y  ( Para limpar pacotes órfãos ou dependências não usadas após a remoção, execute:)

-------------------------------------------------

### **Baixar o docker version 26.0.2 pelo script oferecido pelo rancher**

```bash
curl https://releases.rancher.com/install-docker/26.0.2.sh | sh
```

 <!--(Isso vai baixar e executar o script de instalação fornecido pelo Rancher, que instala o Docker com a versão especificada.)-->

```bash
sudo usermod -aG docker ubuntu
```



```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>

    <link rel="stylesheet" href="css/style.css" />
  </head>

  <body></body>
  <img src="img/BikeSense.svg" alt="" />
</html>
```

---

### Fazer build utilizando o docker

```bash
docker build -t jotapepg/redis:devops .
```

---

## Tipos comuns de commits:

- **feat**: Adição de uma nova funcionalidade.
- **fix**: Correção de um bug.
- **docs**: Alterações na documentação.
- **style**: Mudanças que não afetam o código em si (espaços, formatação, etc).
- **refactor**: Alteração no código que não adiciona nova funcionalidade nem corrige bugs.
- **perf**: Mudança no código que melhora o desempenho.
- **test**: Adição ou correção de testes.
- **build**: Alterações que afetam o sistema de build ou dependências.
- **ci**: Alterações em arquivos de configuração ou scripts de integração contínua.
- **chore**: Tarefas que não se enquadram nos outros tipos (atualizações de dependências, por exemplo).

## Exemplos de commits:

- `feat(homepage): add carousel to highlight new products`
- `fix(cart): correct total calculation on checkout`
- `docs(readme): update project description and instructions`
- `style(navbar): adjust spacing between menu items`
- `refactor(product-page): optimize component rendering`

## Dicas para manter a consistência:

1. **Escopo**: Use um escopo entre parênteses para descrever a parte do código que foi modificada, como um componente, página, ou funcionalidade.
2. **Descrição**: Mantenha a descrição curta e objetiva. Se necessário, adicione uma explicação mais detalhada no corpo da mensagem.
