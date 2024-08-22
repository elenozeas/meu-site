<!DOCTYPE html >
< html  lang =" pt-BR " >
< cabeça >
    < meta  charset =" UTF-8 " >
    < meta  name =" viewport " content =" width=largura-do-dispositivo, escala-inicial=1.0 " >
    < title > Portfólio Pessoal </ title >
    < link  rel =" folha de estilo " href =" style.css " >
</ cabeça >
< corpo >
    <!-- Banner superior transparente com a animação da frase -->
    < div  id =" banner " >
        < div  id =" banner-text " > Bem Vindo ao Portfólio Pessoal </ div >
        < div  id =" botões " >
            < a  href =" pagina1.html " class =" btn " > Página 1 </ a >
            < a  href =" pagina2.html " class =" btn " > Página 2 </ a >
            < a  href =" pagina3.html " class =" btn " > Página 3 </ a >
        </div>​​
    </div>​​

    <!-- Princípio do contêiner -->
    < div  id =" contêiner " >
        <!-- Área central -->
        < div  id =" conteúdo " >
            < h1 > Bem-vindo ao Modelo de Página </ h1 >
        </div>​​
    </div>​​

    < script  src =" script.js " > </ script >
</ corpo >
</ html >


 106 alterações: 106 adições e 0 exclusões106 
estilo.css
Número da linha do arquivo original	Número da linha de diferença	Mudança de linha diferencial
@@ -0,0 +1,106 @@
/* Define margens e preenchimento para zero */
* {
    margem :  0 ;
    preenchimento :  0 ;
    dimensionamento de caixa : caixa de borda;
}

/* Imagem do fundo que cobre toda a página */
corpo {
    imagem de fundo :  url ( 'img01.jpg' );
    tamanho-de-fundo : capa;
    posição de fundo : centro;
    background-repeat : sem repetição;
    família de fontes : Arial , sem serifa;
}

/* Banner superior transparente */
# faixa {
    largura :  100 % ;
    altura :  4cm ;​ /* Altura de 4cm */
    background-color :  rgba ( 255 ,  255 ,  255 ,  0.3 ); /* Transparente */
    posição : fixa;
    topo :  0 ;
    esquerda :  0 ;
    índice z :  10 ;
    estouro : oculto;
    exibição : flex;
    alinhar-itens : centro;
    justificar-conteúdo : centro;
    direção flexível : coluna; /* Alinha o texto e os botões verticalmente */
    preenchimento :  0  10 px ; /* Adiciona um pouco de preenchimento interno */
}

/* Texto no banner */
# texto do banner {
    tamanho da fonte :  3 rem ;
    cor : branco;
    espaço em branco : nowrap;
    posição : relativa;
    animação : slide 10 s linear infinito;
}

/* Animação que move o texto da direita para a esquerda */
@quadros-chave slide {
    0 % {
        transformar :  translateX ( 100 % );
    }
    50 % {
        transformar :  translateX ( 0 % );
    }
    100 % {
        transformar :  translateX ( -100 % );
    }
}

/* Botões dentro do banner */
# botões {
    posição : absoluta;
    fundo :  10 px ;
    direita :  10 px ;
    exibição : flex;
    lacuna :  10 px ;
}

/* Estilo dos botões */
.btn {​
    preenchimento :  10 px  20 px ;
    borda : nenhuma;
    raio da borda :  5 px ;
    cor de fundo :  rgba ( 0 ,  0 ,  0 ,  0.7 );
    cor : branco;
    alinhamento de texto : centralizar;
    decoração de texto : nenhuma; /* Remove o sublinhado dos links */
    cursor : ponteiro;
    transição : cor de fundo 0,3 s ;
}

. btn : pairar {
    cor de fundo :  rgba ( 0 ,  0 ,  0 ,  0.9 );
}

/* Recipiente principal */
# recipiente {
    exibição : flex;
    flex-direction : coluna;
    alinhar-itens : centro;
    margem superior :  4 cm ; /* Espaço abaixo do banner */
}

/* Área central */
# contente {
    alinhamento de texto : centralizar;
    largura :  100 % ;
    altura :  calc ( 100 vh  -  4 cm ); /* Altura total menos o banner */
    exibição : flex;
    flex-direction : coluna;
    alinhar-itens : centro;
    justificar-conteúdo : centro;
}

# conteúdo  h1 {
    cor : branco;
    tamanho da fonte :  2 rem ;
}

