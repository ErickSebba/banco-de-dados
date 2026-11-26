# Banco de Dados

Ambiente de MySQL 8.1 em Docker usado na disciplina de Banco de Dados (UFMT, 2025), com os scripts de criação do banco.

## Estrutura
- `mysql-docker/docker-compose.yml`: sobe o MySQL na porta 3306 (senha de root `admin`, só para uso local).
- `mysql-docker/inicializar/criar.sql`: cria o banco `ufmt` na primeira inicialização.
- `mysql-docker/scripts/criar_tabela_aluno.sql`: cria a tabela `aluno`.
- `mysql-docker/README.md`: passo a passo do Docker e do cliente MySQL.

## Como executar
```
cd mysql-docker
docker-compose up -d
docker exec -it meubanco mysql -uroot -padmin
```
