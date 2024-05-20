**Alteração no Laboratório:**
Devido ao limite diário de adição de colaboradores aos repositórios GitHub, realizamos uma pequena alteração no laboratório para que todas possam realizar a atividade mesmo sem a permissão de colaborador, onde ao invés de clonar diretamente foi adicionado o passo de fork do repositório, onde o clone agora passa a ser do repositório criado pelo fork.
Quem tem a permissão de colaborador e já finalizou a atividade utilizando o clone diretamente não é necessário realizar a atividade novamente!

# Laboratório – Módulo 1: Introdução ao Git e GitHub

Neste laboratório, vamos realizar algumas funções básicas do Git e GitHub. Ao concluir, você terá realizado operações de criação de arquivos e registro de mudanças, assim como submissão e disponibilização deste arquivo dentro de um repositório no GitHub e tudo isso em sua própria Branch. Vamos embarcar!

1. Navegue até o repositório GitHub através deste [link](https://github.com/wesleygomes022/GH4Woman-modulo1)
2. Faça o Fork do repositório 
    1. Clique em Fork do lado direito ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/e4243cb7-857e-4f6f-8ad3-393fdf1624b9)
       (Imagem 1 passo 2 - Print do repositório com seta apontando para o botão fork ao lado direito da tela)
    2. Garanta que em Owner esteja seu usuário selecionado, mantenha as outras opções por padrão e clique em create fork. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/fd570659-a660-4ef4-8a59-207f57526e52)
        (Imagem 2 passo 2 - Tela de criação do Fork) 

3. Clone o Repositório
    1. Vá em Code (ao lado direito da tela) e copie o link HTTPS do repositório criado pelo fork ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/bbb790ad-9fc8-463d-bb3c-7b2f54db5016)
    (Imagem 1  passo 3 - Imagem do repositório com setas apontando para o botão Code e então para o link HTTPS) 

    2. Em seguida, abra um terminal powershell e com o git já instalado em sua máquina e rode o comando `git clone <link copiado>` ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/14dedcee-58fe-46cb-9239-d7761cc59afe)
(lmagem 1 passo 3: Print do terminal com a execução do comando git clone)
    
4. Abra o repositório no MS Explorer e crie um arquivo de texto com a inicial do seu nome e seu sobrenome escrito. Ex: se seu nome for **Geovana Souza**, seu arquivo deve se chamar **gsouza.txt**. ![tela MS Explorer](Images/explorer_I.png)

   (lmagem 1 passo 4: Pasta do repositório clonado apontando para o botão New e então Text Document)
   
![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/fe7451de-428c-4fe5-93bf-bafbebc9155e)
    (Imagem 2 passo 4: arquivo gsouza selecionado na pasta criada)

5. Abra o arquivo *.txt* com seu nome e escreva seu nome completo dentro dele. Após isto, salve (Ctrl + S) e feche o arquivo. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/5508688d-135d-4088-874e-ad434a4b6e4f)
(imagem passo 5: Arquivo de texto criado aberto com o nome "Geovana Souza" escrito dentro dele).

6. Volte ao Powershell. Vá ao diretório do repositório clonado executando cd GH4Woman-modulo1 e então crie uma Branch com o mesmo nome de seu arquivo *.txt* (sua inicial + sobrenome). Faça isto através do comando `git checkout -b <nome-branch>` ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/57729ad7-90a7-4d9b-991b-d2c9632052ae)
(imagem passo 6: print de do terminal da execução do comando de exemplo: git checkout -b gesouza).

7. Execute o comando `git status`: retorna o status de todos os comandos no **working directory** e **staging area**.
    ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/76b59892-cf52-4e2f-8ec4-1807b76e2930)
(imagem passo 7: print de do terminal da execução do comando git status. Comando retornou: On branch gesouza. Untracked files: gsouza.txt)

    > Observe que ele nos retorna que o arquivo foi adicionado ao working directory.

8. Execute o comando `git add <nome-arquivo>`: adiciona o arquivo à staging area. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/b069bc1f-2037-45a4-8565-e8df40733eae)
(imagem passo 8: print do terminal da execução do comando de exemplo: git add gsouza.txt. Comando retorna "Changes to be committed: new file: gesouza.txt)

    > Veja que o mesmo arquivo agora aparece na cor verde e já na staging area.

9. Execute o comando `git commit -m “adicionado arquivo com o meu nome”`: este comando registra as alterações e gera um novo commit como parte do histórico do repositório. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/30a89422-5176-40cf-83b8-39b81f4fee70)
(imagem passo 9: print do terminal da execução do comando de exemplo: git commit -m "adicionado arquivo com o meu nome". Comando retorna: [gesouza dc7f6cf] adicionado arquivo com o meu nome).

10. Execute o comando `git push -u origin <nome-branch>`: este comando irá criar sua Branch remota (no repositório do GitHub) e fará o carregamento deste commit para lá. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/fa6048de-793c-4258-9f1e-e533f982650f)
(imagem passo 10: print do terminal da execução do comando de exemplo: git push -u origin gesouza. O print enfatiza o retorno: To https://github.com/geovanams/GH4Women-modulo1.git. New branch gesouza -> gesouza. branch 'gesouza' set up to track 'origin/gesouza').

11. Navegue até o repositório no GitHub (https://github.com/seuUsername/GH4Woman-modulo1), clique no ícone da *main branch* e selecione sua própria branch. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/a781ca35-ec1a-4642-be62-e5f18af1006c)
(imagem 1 passo 11: Tela do Repositório no Github com seta apontando para o botão main e então seta apontando para o nome da branch gesouza)

    Após isto, você poderá visualizar seu arquivo criado. ![image](https://github.com/GH4WOMAN-M1/GH4Woman-modulo1/assets/50850895/a3839bc6-5697-41c5-8b3b-0df272e8c9f4)

Não é necessário fazer o pull request, pois vamos aprender nas próximas aulas. 🙂

### Parabéns! Você concluiu o laboratório com sucesso! 🎉
