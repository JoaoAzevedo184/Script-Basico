# Script-Basico

Este repositório contém um script em Shell para a criação de estrutura de usuários, diretórios e permissões, desenvolvido como parte do Bootcamp Santander - Linux para Iniciantes.

## Descrição

O script `iac1.sh` implementa a criação de diretórios, grupos de usuários e usuários, além de configurar suas permissões. Ele é útil para configurar um ambiente inicial de trabalho em sistemas Linux, seguindo boas práticas de organização e segurança.

## Funcionalidades

- Criação de diretórios:
  - `/publico`: Diretório público com permissões abertas para todos.
  - `/adm`, `/ven`, `/sec`: Diretórios específicos para grupos administrativos, de vendas e segurança, respectivamente.

- Criação de grupos:
  - `GRP_ADM`: Grupo administrativo.
  - `GRP_VEN`: Grupo de vendas.
  - `GRP_SEC`: Grupo de segurança.

- Criação de usuários:
  - Usuários associados a cada grupo, com diretórios home, shell configurado e senha criptografada.

- Configuração de permissões:
  - Diretórios privados (`/adm`, `/ven`, `/sec`) com acesso restrito aos respectivos grupos.
  - Diretório público (`/publico`) com permissões abertas para todos.

## Como usar

### Pré-requisitos

- Sistema operacional Linux.
- Permissões de superusuário (root) para executar o script.
- O comando `mkpasswd` deve estar disponível no sistema. Caso não esteja, instale o pacote `whois` (disponível na maioria das distribuições Linux).

### Execução do script

1. Clone o repositório:
   ```bash
   git clone https://github.com/JoaoAzevedo184/Script-Basico.git
   ```
2. Acesse o diretório do repositório:
   ```bash
   cd Script-Basico
   ```
3. Dê permissão de execução ao script:
   ```bash
   chmod +x iac1.sh
   ```
4. Execute o script:
   ```bash
   sudo ./iac1.sh
   ```

### O que o script faz?

- Cria os diretórios `/publico`, `/adm`, `/ven` e `/sec`.
- Adiciona os grupos `GRP_ADM`, `GRP_VEN` e `GRP_SEC`.
- Adiciona os usuários com suas respectivas configurações.
- Define as permissões apropriadas para os diretórios.

### Estrutura do código

O script está organizado nas seguintes seções:
1. Criação de diretórios.
2. Criação de grupos de usuários.
3. Criação de usuários e associação aos grupos.
4. Configuração de permissões.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou criar pull requests.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

Se você quiser algo mais personalizado ou precisar de ajustes, me avise!
