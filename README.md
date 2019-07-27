# twebchannel-js
Implementação simples de comunicação com o componente AdvPL TWebChannel.

## Instalação:

```shell
npm install @totvs/twebchannel-js --save
```

## Uso:

#### connect
Inicia a conexão com o TWebChannel AdvPL 

Parametros: 
* callback: Function


```js
    twebchannel.connect(callback);
```

#### jsToAdvpl
Executa uma chamada para a execução do bloco de código **bJsToAdvpl** do TWebChannel AdvPL.

Parametros: 
* key: string
* value: string


```js
    twebchannel.jsToAdvpl("key", "value");
```

#### advplToJs
Função que é executada ao receber uma chamada do metodo **advplToJs** do TWebChannel AdvPL.

Tipo: Function

Parâmetros: 
* key: string
* value: string

```js
    twebchannel.advplToJs = function(key, value) {
        console.log(key, value);
    }
```
