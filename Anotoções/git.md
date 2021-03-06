## Comandos git
####
- git remote add origin git@github.com:<userGitHub>/<nomeDoRepositório>.git ⇾ Cria um "apelido" pro repositório no GitHub. 
  Nesse caso o apelido é Origin, comumente é usado esse nome para o repositório padrão;
- git init ⇾ inicia o git na pasta selecionada;
- git status ⇾ Mostra o status das alterações;
- git add '<nomeDoArquivo>' ⇾ Adiciona o arquivo ao monitoramento de alterações do git;
- git add -A // git add * // git add .⇾ Adiciona todos os arquivos que não estão sendo monitorados ao monitoramento do git;
- git commit -m 'Resumo das alterações' ⇾ commita as alterações para o branch que está sendo trabalhado (ou o branch master, preciso ver ainda);
- git commit -a -m 'Resumo das alterações' ⇾ commita as alterações para o branch que está sendo trabalhado, 
  já adicionando todos os arquivos (tirando a necessidade do git add)
- git branch ⇾ Vê os branchs existentes e sinaliza o que está sendo utilizado no momento com um *;
- git branch <nome> ⇾ Cria um novo branch (não usar os <>);
- git checkout <nome> ⇾ Altera o branch que está sendo usado;
- git diff ⇾ Mostra o que foi alterado antes de dar commit em um arquivo;
- git diff --name-only ⇾ Mostra somente os nomes dos arquivos que foram modificados;
- git checkout HEAD -- <nomeDoArquivo> ⇾ Retorna as atualizações feitas anteriormente no arquivo do branch atual 
  (para selecionar outro branch, só colocar o nome no lugar do HEAD);
- git reset --soft <códigoDoCommit> ⇾ Reseta o arquivo para um commit anterior sem perder o que foi alterado;
- git reset --hard <códigoDoCommit> ⇾ Reseta o arquivo para um commit anterior apagando todas as alterações feitas;
- git reset --mixed <códigoDoCommit> ⇾ Reseta o arquivo para um commit anterior sem perder o que foi alterado, 
  porém é necessário adicionar os arquivos novamente;
- git revert --no-edit <códigoDoCommit> ⇾ Da um commit revertendo o que foi feito no commit especificado. 
  Mudando os arquivos, porém possibilitando "commitar" novamente o mesmo posteriormente;
- git push <apelidoRepositorioGitHub> <nomeBranch> ⇾ Envia o branch selecionado ao repositório GitHub;
- git push <apelidoRepositorioGitHub> :<nomeBranch> ⇾ Deleta o branch do repositório GitHub
- git branch -D nomeBranch ⇾ Deleta o branch local;
- git pull <apelidoRepositorioGitHub> <nomeBranch> ⇾ Recebe o repositório GitHub no branch selecionado;
- git clone <linkRepositorio> ⇾ Clona um repositório do link especificado na pasta selecionada no terminal;
- git remote -v ⇾ Mostra o apelido dos repositório remotos;
