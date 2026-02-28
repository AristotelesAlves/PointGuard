<p align="center">
  <img width="996" height="532" alt="image" src="" />
</p>
<h1 align="center">PointGuard</h1>
<p align="center">
  PointGuard é um microserviço open source em Laravel para gerenciamento de comportamento de usuários em APIs, baseado em regras configuráveis, pontuação, auditoria e controle de acessos.<br>
  Ele é projetado para empresas/organizações, que recebem um token UUID para integrar suas APIs, podendo definir ações como bloqueio, notificação, auditoria e controle de acessos em massa.
</p>
<div align="center">
  
![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/postgresql-%23336791.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

</div>

## Funcionalidades

<p>
  Suporte a múltiplas empresas, cada uma com seu token UUID para integrar a API.
  Configuração de rotas, regras e ações via painel web do microserviço.
  Pontuação automática baseada em comportamento de usuário, incluindo:
  <ol>
    <li>Acessos fora do expediente</li>
    <li>Download ou acesso em massa</li>
    <li>Acesso a rotas restritas</li>
    <li>Falhas repetidas de autenticação</li>
    <li>Uso excessivo de recursos pesados</li>
  </ol>
  Ações configuráveis quando o limite de pontos é atingido:
  <ul>
    <li>Notificação ao usuário</li>
    <li>Bloqueio via hook personalizado</li>
    <li>Apenas bloqueio sem notificação</li>
  </ul>
  Auditoria completa de todos os acessos e ações.<br>
  Banco próprio para armazenar empresas, tokens, regras, pontos e histórico.
</p>

## Como Funciona

<ol>
  <li>Cada empresa cliente recebe um token UUID para integrar a API.
  <li>A empresa configura suas rotas e regras de pontuação pelo painel web do microserviço.
  <li>Define o limite de pontos e a ação desejada ao atingir o limite.
  <li>Cada requisição à API é avaliada pelo microserviço: <br> Pontos são adicionados conforme regras da empresa <br> Ações automáticas são executadas (notificação, bloqueio via hook, etc.)
  <li>Histórico detalhado é armazenado no banco para auditoria.
</ol>

## Contribuição

Contribuições são bem-vindas!

- Fork este repositório
- Crie sua branch `(git checkout -b feature/nome-da-feature)`
- Faça commit das mudanças `(git commit -m 'Adicionar nova feature')`
- Push para a branch `(git push origin feature/nome-da-feature)`
- Abra um Pull Request

## Licença

MIT License © 2026 – Livre para usar, modificar e distribuir.
