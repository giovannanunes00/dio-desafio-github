# dio-desafio-github
### Desafio de Projeto sobre Git/Github
Repositório criado para o desafio de projeto do curso Introdução ao Git e ao GitHub da DIO

## Links Úteis
[Síntaxe Basica Markdown](https://www.markdownguide.org/basic-syntax/)

## 📌 O que é Git vs. GitHub?

* **Git (O Motor):** É um sistema de controle de versão de arquivos **local** e distribuído. Ele roda inteiramente na máquina do desenvolvedor, registrando cada alteração como um "instantâneo" (snapshot) do projeto. Permite rastrear o histórico completo, reverter erros, trabalhar offline e gerenciar múltiplas ramificações (branches) em paralelo com segurança.
* **GitHub (A Nuvem e Colaboração):** É uma plataforma de hospedagem de código baseada em nuvem que integra o ecossistema Git. Ele funciona como o ambiente **remoto** onde as equipes centralizam repositórios, revisam códigos via *Pull Requests*, automatizam fluxos de trabalho (CI/CD), rastreiam problemas (*Issues*) e exibem portfólios profissionais.

---

## 💻 Comandos Essenciais do Git (O Guia de Sobrevivência)

### 1. Configurando o Ambiente
Antes de iniciar os trabalhos, o Git precisa ser "alfabetizado" para saber quem é o autor das alterações:
* `git init`: Inicializa um repositório Git local em uma pasta vazia ou em um projeto existente.
* `git config --global user.name "Seu Nome"`: Vincula seu nome de exibição aos commits.
* `git config --global user.email "seu-email@email.com"`: Vincula seu e-mail aos commits (use o mesmo e-mail do seu GitHub).

### 2. O Ciclo de Trabalho Diário
* `git status`: Exibe o estado atual dos arquivos (mostra o que foi modificado, o que está na fila para salvar e o que o Git ainda não está rastreando).
* `git add <nome-do-arquivo>`: Envia um arquivo específico para a área de preparação (*Staging Area*).
* `git add .`: Adiciona **todas** as modificações da pasta atual para a *Staging Area*.
* `git commit -m "tipo: mensagem curta"`: Registra permanentemente as alterações salvas na *Staging Area* criando um ponto na história do projeto.
* `git push origin <nome-da-branch>`: Envia os commits da sua máquina para o repositório remoto no GitHub.
* `git pull origin <nome-da-branch>`: Baixa as atualizações mais recentes do servidor remoto e as mescla na sua máquina, garantindo que seu código local não fique desatualizado.

### 3. Ramificações (Branches) e Organização
Trabalhar em branches evita que alterações experimentais quebrem a linha principal de produção (`main` ou `master`):
* `git branch`: Lista todas as branches locais existentes no projeto.
* `git checkout -b <nome-da-nova-branch>`: Cria uma nova ramificação de trabalho e muda para ela imediatamente.
* `git checkout <nome-da-branch>`: Alterna entre branches existentes.
* `git merge <nome-da-branch>`: Une o histórico de alterações da branch especificada para a ramificação onde você está posicionado agora.

---

## 🛠️ Boas Práticas e Padrões Profissionais
No dia a dia técnico, a clareza do histórico é fundamental. Adoto o padrão de **Commits Semânticos (Conventional Commits)** para manter o projeto legível por qualquer membro da equipe:

* `feat:` Uma nova funcionalidade ou recurso adicionado ao projeto.
* `fix:` Correção de um bug ou comportamento inesperado.
* `docs:` Alterações exclusivas na documentação (como criar ou atualizar o README).
* `style:` Ajustes visuais ou de formatação que não alteram a lógica do código (espaços, identação, chaves).
* `refactor:` Alterações de código que melhoram sua estrutura interna (limpeza de código) sem alterar o comportamento final.
* `test:` Criação ou modificação de scripts de testes (manuais ou automatizados).

## 🎓 Conclusão e Objetivos
O domínio do Git e do GitHub é um pilar indispensável para atuar com eficiência em equipes ágeis, garantindo a rastreabilidade do código, o versionamento correto de scripts de automação e a segurança da base de código do produto.
