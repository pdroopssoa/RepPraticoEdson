# RepPraticoEdson

# Git Branching - Comandos Essenciais

# 1. Ver todas as branches (locais e remotas)
git branch            # Somente locais
git branch -r         # Somente remotas
git branch -a         # Todas (local + remota)

# 2. Criar uma nova branch
git branch nome-da-branch

# 3. Trocar para uma branch existente
git checkout nome-da-branch

# 4. Criar e já trocar para a nova branch
git checkout -b nome-da-branch

# 5. Renomear uma branch
git branch -m novo-nome            # Estando nela
git branch -m antigo novo-nome     # Especificando

# 6. Deletar uma branch local
git branch -d nome-da-branch       # Só se já foi mesclada
git branch -D nome-da-branch       # Forçar deletar

# 7. Subir uma branch para o repositório remoto
git push origin nome-da-branch

# 8. Buscar (fetch) todas as branches remotas
git fetch

# 9. Criar uma branch local rastreando uma remota
git checkout -b nome-local origin/nome-remoto

# 10. Associar branch local a uma remota (set upstream)
git push -u origin nome-da-branch

# 11. Ver em qual branch você está
git status
git branch --show-current

# 12. Listar todas as branches com info de tracking
git branch -vv

# 13. Atualizar informações do remoto
git remote update

# 14. Remover referência a branches remotas deletadas
git remote prune origin

# 15. Mesclar uma branch na atual
git merge nome-da-branch

# 16. Resolver conflitos após merge
# (Feito manualmente nos arquivos + depois:)
git add .
git commit

# 17. Rebase interativo (avançado)
git rebase -i nome-da-branch

# 18. Clonar um repositório (inclui todas as branches)
git clone url-do-repo

# 19. Ver detalhes do repositório remoto
git remote -v

# 20. Adicionar um repositório remoto (se ainda não houver)
git remote add origin url-do-repo

# 21. Mudar a URL do repositório remoto
git remote set-url origin nova-url


