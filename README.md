# Cursos

Sistema WEB para ministrar cursos

# Etapas

## Infraestrutura
[x] Servidor com HTTPS na Digital Ocean
[x] Projeto com Laravel Sail
[x] Repositório no Github
[x] Banco de Dados
[ ] Deploy com Github Actions
[ ] Telescope com debgbar
[ ] Log de Erros enviados para E-mail
## Funcionalidades
[ ] Cadastro e Autenticação dos Usuários
[ ] CRUD de Cursos
[ ] CRUD de Aulas dentro dos Cursos
[ ] CRUD de Anexos dentro das Aulas
[ ] Estudar curso
[ ] Anotações do Aluno
[ ] Aula com opção de vídeo
[ ] Aula com opção de questões de multipla escolha
[ ] Chat entre todos Usuários
[ ] Chat entre os Alunos de um mesmo curso
[ ] Chat privado

## Entidades

### Usuário
- nome
- email
- senha
- foto

### Curso
- professor(fk:Usuario)
- nome
- descricao
- imagem

### Aula
- curso(fk:Curso)
- titulo
- texto
- imagem
- video
- audio
- pdf

### Anexo
- aula(fk:Aula)
- titulo
- tipo
- path

### Chat
- remetente(fk:Usuario)
- destinatario(fk:Usuario)
- mensagem
- visualizada
