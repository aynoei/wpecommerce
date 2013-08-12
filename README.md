Módulo de integração para WordPress/WP e-Commerce
=================================================
---
Descrição
---------
---

Com o módulo instalado e configurado, você pode pode oferecer o PagSeguro como opção de pagamento em sua loja. O módulo utiliza as seguintes funcionalidades que o PagSeguro oferece na forma de APIs:

 - Integração com a [API de Pagamentos]
 - Integração com a [API de Notificações]

 
 Requisitos
----------
---
 - [WordPress] 3.5.2
 - [WPeCommerce] 3.8.12.1
 - [PHP] 5.3.9+
 - [SPL]
 - [cURL]
 - [DOM]
 
 
 Instalação
----------
---
 - Certifique-se de que não há instalação de outros módulos para o PagSeguro em seu sistema;
 - Baixe o repositório como arquivo zip ou faça um clone;
 - No menu da pagina de administrador vá em Plugins-> Add New em Upload e selecione o zip do módulo do PagSeguro para fazer a instalação no WordPress, após a instação selecione a opção Active. Esta instalação não afetará nenhum arquivo do seu sistema, somente adicionará os arquivos do módulo PagSeguro;
 - Certifique-se de que as permissões das pastas e arquivos recém copiados sejam, respectivamente, definidas como 755 e 644;
 
 
 Configuração
------------
---
Para acessar e configurar o módulo acesse o menu WPeCommerce -> Settings -> Store -> Payments -> PagSeguro Oficial[settings]. As opções disponíveis estão descritas abaixo.

 - **Enable/Disable**: ativa/desativa o módulo.
 - **Title**: Titulo a ser exibida na tela de Pagamento.
 - **Description**: Descrição a ser exibida na tela de Pagamento.
 - **Email**: email gerado no PagSeguro.
 - **Token**: token gerado no PagSeguro.
 - **Url Redirect**: ao final do fluxo de pagamento no PagSeguro, seu cliente será redirecionado automaticamente para a página de confirmação em sua loja ou então para a URL que você informar neste campo. Para ativar o redirecionamento ao final do pagamento é preciso ativar o serviço de [Pagamentos via API]. Obs.: Esta URL é informada automaticamente e você só deve alterá-la caso deseje que seus clientes sejam redirecionados para outro local.
 - **Url Notification**: sempre que uma transação mudar de status, o PagSeguro envia uma notificação para sua loja ou para a URL que você informar neste campo. Obs.: Esta URL é informada automaticamente e você só deve alterá-la caso deseje receber as notificações em outro local.
 - **Invoice Prefix**: Prefixo para controle das transações realizadas com o PagSeguro.
 - **Charset**: codificação do seu sistema (ISO-8859-1 ou UTF-8).
 - **Debug Log**: ativa/desativa a geração de logs.
 - **diretório**: informe o local a partir da raíz de instalação do WordPress onde se deseja criar o arquivo de log. Ex.: /logs. Caso não informe nada, o log será gravado dentro da pasta ../PagSeguroLibrary/PagSeguro.log.


 Changelog
---------
---
1.0

 - Versão inicial. Integração com API de checkout e API de notificações.
 
 
 Licença
-------
---
Copyright 2013 PagSeguro Internet LTDA.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.


Notas
-----
---
 - O PagSeguro somente aceita pagamento utilizando a moeda Real brasileiro (BRL).
 - Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial.
 - Certifique-se que tenha definido corretamente o charset de acordo com a codificação (ISO-8859-1 ou UTF-8) do seu sistema. Isso irá prevenir que as transações gerem possíveis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
 - Para que ocorra normalmente a geração de logs, certifique-se que o diretório e o arquivo de log tenham permissões de leitura e escrita.


[Dúvidas?]
----------
---
Em caso de dúvidas mande um e-mail para desenvolvedores@pagseguro.com.br


Contribuições
-------------
---
Achou e corrigiu um bug ou tem alguma feature em mente e deseja contribuir?

* Faça um fork.
* Adicione sua feature ou correção de bug.
* Envie um pull request no [GitHub].


  [API de Pagamentos]: https://pagseguro.uol.com.br/v2/guia-de-integracao/api-de-pagamentos.html
  [API de Notificações]: https://pagseguro.uol.com.br/v2/guia-de-integracao/api-de-notificacoes.html
  [Dúvidas?]: https://pagseguro.uol.com.br/desenvolvedor/comunidade.jhtml
  [Pagamentos via API]: https://pagseguro.uol.com.br/integracao/pagamentos-via-api.jhtml
  [Notificação de Transações]: https://pagseguro.uol.com.br/integracao/notificacao-de-transacoes.jhtml
  [WordPress]: http://wordpress.org/
  [WPeCommerce]: http://getshopped.org/
  [PHP]: http://www.php.net/
  [SPL]: http://php.net/manual/en/book.spl.php
  [cURL]: http://php.net/manual/en/book.curl.php
  [DOM]: http://php.net/manual/en/book.dom.php
  [GitHub]: https://github.com/pagseguro/wpecommerce/