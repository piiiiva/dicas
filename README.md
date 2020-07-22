<h1 align="center"> 
    Como remover o node_modules do seu repositório no Github
</h1>

<p>
  <b>1.</b> Acessar a raiz do projeto pelo terminal.
</p>
<p>
  <b>2.</b> Criar o arquivo .gitignore e adicionar na raiz do projeto se não existir.
</p>

<p>
  <b>3.</b> Dentro do arquivo .gitignore, adicionar o que você quer que seja ignorado, nesse caso a pasta node_modules.
</p>

`node_modules`

&nbsp;

<p>
  <b>4.</b> Remover a pasta node_modules do repositório via terminal
</p>

`git rm -r --cached node_modules`

<p>
 <b>5.</b> Você pode conferir se os arquivos foram deletados.
</p>

`git status`

<p>
  <b>6.</b> Fazer um commit do repositório sem a pasta node_modules
</p>

`git commit -m "Removed node_modules folder"`

<p>
  <b>7.</b> Fazer um push com as alterações para o github
</p>

`git push origin master`

&nbsp;

<p>
  <b>8.</b> Adicionar o .gitignore no repositório, fazer um commit e enviar para o github.
</p>

`git add .gitignore`

`git commit -m "Updated .gitignore file"`

`git push origin master`

&nbsp;
<p>
  <b>Obs:</b> Serve para arquivos como package-lock.json também.
</p>
