# twebchannel-js

> Implementação simples de comunicacao com o componente AdvPL TWebChannel

## Instalação:

```shell
npm install @totvs/twebchannel-js --save
```

## Uso:

### Métodos

#### connect
Inicia a conexão com o TWebChannel AdvPL 

Parametros: 
* callback: Function


```js
    twebchannel.connect(callback);
```

#### jsToAdvpl
Executa uma chamada para a execucao do bloco de codigo **bJsToAdvpl** do TWebChannel AdvPL.

Parametros: 
* key: string
* value: string



```js
    twebchannel.jsToAdvpl("key", "value");
```

### Propriedades

#### advplToJs
Funcao que é executada ao receber uma chamada do metodo advplToJs

Tipo: Function

Parametros: 
* key: string
* value: string

```js
    twebchannel.advplToJs = function(key, value) {
        console.log(key, value);
    }
```
