# PHONEGAP
É uma plataforma de desenvolvimento mobile *HIBRIDA*. É da Adobe, existe desde 2012 e é gratuita e *OPEN SOURCE*.
O desenvolvimento é hibrido porque ela exporta para até 9 plataformas diferentes (Sistemas Operacionais Mobile)
> `Android, iOS, WindowsPhone, BlackBerry, Tizen, Bada, FireFoxOS, AmazonOS.`


Podemos fazer um site que vai ser compilado e transformado em *APLICATIVO* graças ao *PHONEGAP*.
(Nunca colocar o nome do projeto ou páginas em *MAIUSCULO*, sempre em minusculo. Nomes em maisculo podem não ser lidos corretamente pelo compilador)

## INSTALAÇÃO
Para fazer a instalação do PhoneGap é necessário instalar o Node.js antes.
Com o Node instalado execute o comando no Prompt: 

> `npm install -g phonegap`

Para criar um aplicativo execute o comando (Lembre-se de conferir se está na pasta desejada para criação do projeto):

> phonegap create `<nome do aplicativo>`


## CORDOVA
O Cordova é o coração do PhoneGap, ele é o compilador, motor de execução, kernel do PhoneGap. Só conseguimos criar aplicativos graças ao *CORDOVA*, existem diversas plataformas que rodam em cima do *CORDOVA*
`PhoneGap, Ionic, Intel XDK`


Compatibilidade 100% porque usam o mesmo *KERNEL (CORDOVA)*
*RATCHET*
É uma folha de estilos com uma biblioteca gratuita, OpenSource e da mesma equipe que criou o BOOTSTRAP


### PADRÃO APP EM HTML
>* `<html>` 
>   * `<head>`
>       * <title></title>
>   * `</head>`
>   * `<body>`
>       * <header/> = cabeçalho do app 
>       * <section/> = conteúdo do app
>       * <footer/> = rodapé do app
>       * <script/> = JavaScript e importações de bibliotecas
>   * `</body>`
>* `</html>`

### JQUERY
Javascript é um trabalho muito chato e braçal, para amenizar isso utilizaremos a biblioteca *JQUERY*. Sempre importar no final da página (antes de fechar o `<body>`)
Comandos iniciados por "$" significa um comando em JQuery
Comandos com "#" significa que estamos nos referindo à ID de algum objeto da página


Importar JQuery
Para usar o serviço pré-pronto é preciso fazer uma chamada remota do script do JQuery
`<script src="js/jquery-3.0.0.min.js"></script>`


Importar Script de tabela automática do JQuery
Para poder carregar GRIDS de forma automática (SIMPLES) importe uma bibliotca de templates do JQuery
`<script src="js/jquery.tmpl.min.js"></script>`




## #AJAX
É a tecnologia utilizada para interagir o APP com o SERVIÇO (Azure com App)

>$.ajax({
>	    url: url do serviço,
>	    type: tipo de processo (GET, POST),
>	    success: caso a conexão dê certo,
>	    error: caso a conexão falhe
>	    });


Quando se tratar de enviar dados para o .ajax, certifique de não estar usando a tag `<form>`, ele não reconhecerá. Use apenas a tag `<div>`
*DEBUGGER*
Para monitorar um código JS no navegador utilizamos o comando debugger; onde você quer que o código pare, teste o app no Google Chrome com a aba de Console aberta (F12). Esse processo equivale à um Breakpoint.
#### FORMAS DE TESTAR O APLICATIVO

>01) Chrome
>Pelo navegador
>02) Simulador do PhoneGap
>É preciso ligar o servidor do phonegap via prompt de comando:
>phonegap serve


E baixar o aplicativo da PhoneGap. O notebook ou desktop rodando o servidor e o celular para teste devem estar na mesma Rede (WIFI) para que se encontrem.
Para ligar o servidor é preciso estar na mesma pasta do aplicativo (cd <pasta_do_app>)
Visualizamos em tempo real as telas do aplicativo na hora.
03) Compilar o aplicativo (gerar um .APK - binário do android)
É preciso criar uma conta na ADOBE
https://build.phonegap.com/


Zipar a pasta do seu aplicativo (Geralmente é a pasta www) e dar upload do arquivo zipado no site. Será gerado um QRCode onde você vai poder estar baixando seu projeto .apk e instalando no seu dispositivo.