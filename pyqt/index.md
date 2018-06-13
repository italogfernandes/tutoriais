# Tutoriais
Tutorias com finalidade de ensino do uso de ferramentas de programação (Git, Atom, etc).

## Git Bash + Atom

### Como criar um novo repositório

* Abra sua página do [GitHub](www.github.com) e no canto superior direito clique no pequeno botão de **+**, então selecione `New repository`:

![Imagem do GitHub Create1](imgs/github_create_repo_1.png)

* Preencha:
    * **Name**: Nome do seu repositório (que também será o link para ele).
    * **Description**: É opcional mas recomendado adicionar uma descrição.
    * **Privacidade**: Toda conta GitHub pode criar repositórios públicos, mas caso deseje é possível ativar a opção de repositório privados. Estudantes podem ter repositórios privados ilimitados caso requisitem seu [student developer pack](https://education.github.com/pack).
    * **README**: O GitHub oferece a opção de inicializar seu repositório com um arquivo README em formato [https://guides.github.com/features/mastering-markdown/](Markdown), este arquivo é onde iremos descrever nosso repositório.
    * **.gitignore**: Este arquivo serve para dizer quais tipos de arquivos o git deve ignorar ao analisar seu projeto. Por exemplo, se você programa em python não é recomendado rastrear a versão de arquivos de cache (*__pycache__/*) dos seus pacotes, pois eles vão apenas dar volume e atrapalhar no gerenciamento das versões do seu projeto.
    * **License**: É uma boa prática colocar alguma licença open-source sobre o seu código, isso dirá quais as permissões que quem tiver acesso a ele terá. Leia mais em [choosealicense.com](https://choosealicense.com/licenses/)

![Imagem do Create2](imgs/github_create_repo_2.png)

* MIT License File:

![Imagem do GitHub License](imgs/github_create_repo_license.png)

* .gitignore para python.

![Imagem do GitHub GitIgnore](imgs/github_create_repo_git_ignore.png)

### Clonando o repositório para seu computador

* Com o repositório criado, clique em **Clone or download** e selecione a sua opção de download (HTTPS ou [SSH](https://help.github.com/articles/connecting-to-github-with-ssh/)), na opção https será requisitada suas credenciais para realizar um push, selecione o copie o endereço que aparecerá.

![Imagem do GitHub Clone Http](imgs/github_create_repo_clone_http.png)

* Selecione uma pasta no seu computador e clique com o botão direito em um espaço vazio.

![Imagem do GitBash1](imgs/git_bash_1.png)

* No terminal aberto digite `git clone https://github.com/<username>/<repository_name>.git` e pressione enter para executar o comando.

![Imagem do GitBash  Clone](imgs/git_bash_clone.png)

* Uma nova pasta será criada com o nome do seu repositório e os arquivos presente nela serão clonados para seu computador. (A pasta .git é utilizada pelo sistema para gerenciar as versões do seu projeto)

![Imagem do GitBash  Clone Success](imgs/git_bash_clone_success.png)

### Usando o Atom

* Abra o Atom e selecione **Open Folder**. Navegue até a pasta que você clonou do GitHub e selecione-a.

![Imagem do Atom Open](imgs/atom_open_proj.png)

* Sua pasta aparecerá no Atom com um ícone de repositório, caso você editar algum arquivo ele ficará destacado, verde para arquivos novos, amarelo para arquivos modificados e vermelho para arquivos excluídos.

![Imagem do Atom Git Edited](imgs/atom_git_edited_files.png)

* Todos as ferramentas do Atom podem ser acessadas digitando `Ctrl+Shift+P` e pesquisando pelo nome da ferramenta.

![Imagem do Atom Ctrl Shift P](imgs/atom_ctrl_shift_p.png)

* Um exemplo é o Preview de arquivos formatados com markdown.

![Imagem do Atom Markdown Preview](imgs/atom_markdown_preview.png)

* Para acessar o painel do Git, você pode pesquisar por `Git Tab` na paleta de comandos, acessar o **menu View** ou então clicar no pequeno ícone no **canto inferior direito** onde está escrito a quantidade de arquivos modificados.

![Imagem do Atom Git Tab Cmd](imgs/atom_ctrl_shift_p_git_tab.png)

* Este painel é dividido em 3 partes:
    * **Unstaged Changes**: Suas modificações em geral.
    * **Staged Changes**: As modificações que você selecionou para salvar em um Commit.
    * **Commits**: Uma entrada de texto onde você pode inserir uma mensagem e criar um novo commit e a lista de commits deste repositório.

![Imagem do Atom Git Tab](imgs/atom_git_tab.png)

* Após realizar alguma modificação selecione os arquivos que deseja dar um "Stage", isso equivale ao comando `git add <nome_do_arduino>`. Digite uma mensagem que descreva brevemente suas modificações.

![Imagem do Atom Git Tab Commit](imgs/atom_git_commit.png)

* Clique em commit to master e seu commit aparecerá na lista, note também o surgimento de um número próximo a palavra **Push** no inferior da tela. O comando `git push` envia suas modificações para o repositório online do GitHub (sua origin). Este comando se complementa com o `git  pull` que busca os commits não estão no seu computador (remote).

![Imagem do Atom Git Tab Push](imgs/atom_git_push.png)

* Depois do push você poderá ver suas modificações no endereço do repositório online.

![Imagem do Atom GitHub After Push](imgs/git_hub_after_push.png)

### Configurando uma GitHub Page

Acesse para saber mais sobre o [GitHub Pages](https://pages.github.com/).

* No seu repositório acesse o menu de configurações.

![Imagem do Atom GitHub Page Settings](imgs/git_hub_page_settings.png)

* Navegue até a parte que configura o GitHub Pages. Selecione de qual arquivo você deseja que GitHub gere sua página e salve. Ela já estará disponível em `username.github.io/repositoryname`, para ficar mais agradavél a vista selecione um tema.

![Imagem do Atom GitHub Page Source](imgs/github_pages_source_and_theme.png)

* Alguns exemplos de temas disponíveis.

![Imagem do Atom GitHub Page Theme](imgs/github_pages_theme_selection.png)

* Link onde minha página foi publicada.

![Imagem do Atom GitHub Page Publish](imgs/github_pages_publication.png)

## Autor

* Ítalo Fernandes - [italogfernandes.github.io](https://italogfernandes.github.io)
