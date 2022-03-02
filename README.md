<div>
    <h1 align="center">Espaço de estudo</h1>
    <p align="center">Essse repositório é destinado ao simples registro de anotações e aplicações do meu estudo de DevOps.</p>
</div>

<div>
    <h1 align="center">Alguns comandos docker</h1>
    <table align="center">
    <tr align="center">
        <td ><b>Comando</b></td>
        <td ><b>Descrição</b></td>
    </tr>
    <tr>
        <td>docker rmi $(docker image ls -aq) --force</td>
        <td>Remove todas os containers com as tags <b><i>-aq</i><b> e caso tenha algum container sendo utilizado por algum serviço que o docker não consiga remover.<br> A tag <b><i>--force</i></b>, força a remoção da imagem.</td>
    </tr>
    <tr>
        <td>docker build -t "Nome-de-usuário-no-Docker-Hub"/Nome-da-imagem</td>
        <td>Cria imagem com o nome de usuário do Docker Hub.</td>
    </tr>
    <tr>
        <td>docker ps -s</td>
        <td>A flag <b><i>-s</i></b> mostra uma coluna com o tamanho da imagem.</td>
    </tr>
    <tr>
        <td>docker history "nome-da-imagem"</td>
        <td>Apresenta doversas informações sobre a imagem.</td>
    </tr>
    <tr>
        <td>docker run -it --mount type=bind,source=/home/devops/devops-applications/app-exemplo,target=/app ubuntu bash</td>
        <td>Persiste dados com <b><i>bind mount</i></b>. Nesse caso os <i>bind mount</i> depedem da estrutra de pastas do host.<br> Precisamos passar um local de armazenamento no nosso host.</td>
    </tr>
    </tr>
        <tr>
        <td>docker run -it -v "nome do volume":/app ubuntu bash</td>
        <td>Persistindo dados com VOLUME.<br> Os volumes são gerenciados pelo Dokcer.</td>
    </tr>
    <tr>
        <td>docker run -it --mount source=volume-1,target=/app ubuntu bash</td>
        <td>Persistindo dados com MOUNT.</td>
    </tr>
    <tr>
        <td>docker run –it --mount type=tmpfs,detination=/app ubuntu bash</td>
        <td>Memória temporária no meu host com o TMPFS, que armazena dados em memória volátil.</td>
    </tr>
    <tr>
        <td>docker inspect "ID do container"</td>
        <td></td>
    </tr>

</table>

</div>

###Teste "git stash"





