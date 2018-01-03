# bower # 
> Também é um gerenciador de pacotes como o npm porém focado no frontend

Inspirado no [vídeo](https://www.youtube.com/watch?v=R7CWXUwaKVA) do [Rafael Dias](https://github.com/eudiasrafael)

## Instalação ##
* `npm install -g bower`

## Iniciando ##
* `bower unit`
* name: `bower`
* description: `Gerenciando pacotes do frontend com Bower`
* main file: `index.html`
* keywords: `Bower` `initBower` `startBower`
* authors: `Mir Carvalho <deppbrazil@gmail.com>`
* license: `MIT`
* homepage: `https://github.com/deppbrazil/bower` 
* set currently installed components as dependencies?: `yes`
* add commonly ignored files to ignore list?: `yes`
* would you like to mark tis package as private which prevents it from being accidentally published to the registry?: `yes`

Isso vai gerar o [bower.json](https://github.com/deppbrazil/bower/blob/master/bower.json)

* [Documentação](https://bower.io/docs/api/#init)

## Buscando pacotes/plugin pela linha de comando ##
* `bower search nomeDoPacote`
* [Documentação](https://bower.io/docs/api/#search)

## Buscando pacotes/plugin pela Web ##
* [Site oficial do Bower](https://bower.io/search/)

## Ver informações do pacote ##
* `bower info nomeDoPacote`

## Instalação de um pacote ## 
* `bower install nomeDoPacote`
* `bower install nomeDoPacote@123` instala na versão específicada 

## [Salvando dependências]() ##
* `bower install --save nomeDoPacote`
## Salvando dependências de desenvolvimento ##
* `bower install --save-dev nomeDoPacote`

## Instalando dependências ## 
* `bower install` instala todas as dependências
## Instalando dependências de produção ## 
* `bower install --production` instala apenas as dependências de produção
* [Documentação](https://bower.io/docs/api/#install)

## Atualizando pacotes ##
* `bower update nomeDoPacote`
* `bower update --save nomeDoPacote` salva no bower.json

## Removendo um pacote ## 
* `bower uninstall nomeDoPacote`
* `bower uninstall --save nomeDoPacote` para salvar no `bower.json`
* `bower uninstall --save-dev nomeDoPacote` para salvar no `bower.json`
>remove os pacotes e suas dependências, exceto se a dependência também é de outro pacote.

## [Ver pacotes instalados no projeto]() ##
* `bower list`
> Além de listar os pacotes ele verifica se tem alguma nova versão disponível do pacote e também informa `extraneous` se caso ele não estiver listado como dependência.

## Cache ##
* `bower cache list` lista pacotes cacheados 
* `bower cache clean` limpa cache

## Sufixos de versões ## 
* `*` versão mais recebte - mantém a versão mais recente 
* `123` versão exata - mantém exatamente a versão específicada
* `~123` versão aproximada - mantém sempre a versão menor somente permitindo alterações no ultimo parâmetro de versionamento 12`3`(permite bugFixes)
* `^123` compatível com - sempre aceita mudanças de versões menores, mas nunca permite versões novas de sistema 1`23` (permite newFeatures ou bugFixes)
* `>123` maior que - mantém sempre versões maiores que a específicada, é mesma função do `*`
* `>=123` maior igual que - matém sempre versões maiores ou iguais que a específicada, é mesma função do `*`
* `<123` menor que - mantém sempre versões menores que a específicada, ou seja neste caso pegaria a `1.2.2`
* `<=123` menor igual que - matém sempre versões menores ou iguais que a específicada, é mesma função da `versão exata`

* `^123` mais usada =)

[Documentação de Sufixos](https://semver.org/lang/pt-BR)