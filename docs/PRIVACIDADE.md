# Política de privacidade — ROMFlow

Revisada em 25 de novembro de 2026 · válida para os fluxos da versão 0.1.24

## Quem desenvolve o aplicativo

ROMFlow é um projeto independente de Técnico Root, de Ivanildo Sousa. Não é um produto oficial nem possui vínculo declarado com Motorola, Lenovo, Samsung ou Google. Contato de suporte e privacidade: [paradaseimportsoficial@gmail.com](mailto:paradaseimportsoficial@gmail.com).

## Para que os dados são usados

O aplicativo permite consultar o catálogo Motorola/Lenovo e baixar o pacote de firmware indicado pelo serviço. O modelo e o IMEI podem ser digitados pelo usuário ou lidos por USB/OTG, e são enviados ao serviço Motorola/Lenovo para identificar o aparelho e consultar os pacotes. O app pode ler modelo e IMEI de outro Motorola conectado por USB/OTG em fastboot, quando você seleciona essa opção e autoriza o acesso USB no Android. A leitura é apenas de identificação, sem gravação, apagamento ou reinício; o número completo não aparece na tela de leitura. Ao tocar em Consultar, esses dados são enviados ao serviço Motorola/Lenovo e usados somente em memória, sem histórico ou envio ao criador e aos anúncios. Se o bootloader não informar os dados necessários, complete os campos manualmente. Use apenas identificadores de aparelhos próprios ou cujo titular tenha autorizado a consulta.

## Sugestão automática do modelo sem root

Ao abrir o aplicativo, o ROMFlow tenta ler o código do modelo XT do próprio celular por informações do sistema Android, sem root e sem consultar o IMEI automaticamente por esse fluxo. O modelo é sugerido no campo editável da consulta, somente se estiver vazio. Ele permanece em memória e só é enviado à Motorola/Lenovo quando você confirma a consulta. Se o Android não fornecer um XT válido, complete manualmente. Você pode substituir o modelo para consultar outro aparelho.

## Leitura opcional com root — edição do GitHub

Na tela de consulta, Ler este celular com root permite tentar ler modelo e IMEI do próprio aparelho. É opcional: não solicita root na inicialização e só tenta a leitura ao tocar em Ler dados com root. A autorização e a revogação são feitas pelo gerenciador de root. Os comandos são fixos e somente de leitura; não há terminal persistente, logs com identificadores ou histórico desses dados. O IMEI aparece mascarado na conferência. Ao confirmar Consultar, os dados são enviados à Motorola/Lenovo. Pode ser necessário completar manualmente mesmo com root. A função não instala a ROM no próprio celular. A edição para loja não contém essa função.

## Conta, login e sessão

O login padrão abre o navegador externo na página Motorola/Lenovo, incluindo o acesso por conta Google. O código nativo do aplicativo não lê nem registra os campos de senha dessas páginas. Após o login, o aplicativo recebe um código de retorno, valida a sessão e guarda os dados técnicos necessários para reutilizá-la, criptografados com Android Keystore. O navegador pode manter seus próprios cookies e a sessão Google/Lenovo. Sair do aplicativo não encerra automaticamente as sessões no navegador.

## Armazenamento no aparelho

O modelo e o IMEI digitados ficam na memória durante o fluxo de consulta; o app não os grava deliberadamente em preferências, arquivos de histórico ou relatórios do criador. As respostas do catálogo também são processadas em memória. O aplicativo guarda localmente a sessão criptografada, preferências, metadados e progresso dos downloads e dados de controle de atualização e publicidade. Os endereços temporários dos novos downloads são criptografados com Android Keystore. O backup automático desses dados do app está desabilitado. O Android mantém os arquivos de Downloads e pode conservar registros dos downloads antigos feitos pelo seu gerenciador.

## Idioma do aplicativo

A preferência de idioma é guardada localmente; no Android 13 ou superior, o sistema também pode gerenciá-la. As traduções acompanham o APK e funcionam sem conexão. A troca de idioma não envia textos, identificadores ou sessões a serviços de tradução.

## Downloads de ROM

Os novos downloads são feitos diretamente do endereço fornecido pelo catálogo por um serviço do ROMFlow em primeiro plano, com notificação. Downloads antigos realizados pelo gerenciador do Android continuam sob seu controle. As ROMs ficam em Downloads/ROMFlow e podem continuar no aparelho após a desinstalação do app. Ao conectar aos serviços, os servidores de destino recebem dados técnicos da conexão, como endereço IP. O criador não hospeda as ROMs nem mantém um servidor próprio para receber modelo, IMEI ou sessão.

## Extração e instalação por USB/OTG

O recurso de instalação lê os arquivos da ROM e os checksums na pasta escolhida. Com sua autorização, consulta produto e número de série do aparelho conectado por USB/OTG; a tela mostra apenas o final da identificação. A preparação temporária e o registro da última execução ficam privados no celular controlador e não são enviados ao criador nem ao SDK de anúncios pelo código do app. A preparação temporária é removida após a execução. Os arquivos extraídos e scripts exportados permanecem na pasta escolhida, inclusive após desinstalar. Limpar os dados do app remove o registro privado. A instalação grava partições do outro aparelho e pode apagar seus dados conforme a opção escolhida; faça backup.

## USB avançado e instaladores

Ao selecionar uma pasta e instalador BAT/SH/XML, imagem ou ZIP, o aplicativo pode preparar cópias temporárias privadas dos arquivos necessários antes de enviá-los ao outro aparelho por USB autorizado. As cópias são removidas após o encerramento; interrupções do processo podem deixá-las até a limpeza posterior. O resultado mais recente da execução fica salvo localmente. Esses arquivos não são enviados ao criador ou aos anúncios por esse fluxo.

## Publicidade e escolhas de privacidade

O app integra Google Mobile Ads (AdMob) e User Messaging Platform (UMP). A edição de desenvolvimento usa anúncios de demonstração. As edições assinadas de distribuição usam a unidade publicitária do criador, sujeita à disponibilidade e autorização de veiculação da plataforma. O SDK pode tratar identificadores de publicidade/dispositivo, endereço IP, dados de interação com anúncios, diagnóstico e informações técnicas do aplicativo. A configuração de privacidade e a região podem afetar a forma de tratamento e a personalização. Modelo, IMEI e sessão Motorola informados no fluxo de consulta não são repassados pelo código do aplicativo ao SDK de publicidade. O Google pode fornecer ao criador relatórios agregados de publicidade.

## Consentimento e opções

O UMP consulta o estado de consentimento e apresenta as mensagens configuradas pelo publicador quando aplicáveis. O app só solicita anúncios quando o UMP informa que isso é permitido. Quando exigida, a entrada Opções de privacidade dos anúncios aparece em Sobre. As preferências de identificador de publicidade também podem ser geridas nas configurações do Android. A ROM permanece acessível quando um anúncio não está disponível; não há pagamento ou anúncio obrigatório para liberar o arquivo salvo.

## Atualizações do aplicativo

Na edição para distribuição direta, a verificação de novas versões consulta o GitHub e o download de uma atualização usa o serviço indicado na publicação. O GitHub recebe dados normais da conexão. Na atualização 0.1.21, a cópia do APK conferida para instalação pode permanecer no cache privado. Cópias com mais de sete dias são removidas quando ocorre uma nova verificação; também podem ser removidas pela limpeza dos dados/cache do app ou pelo Android. Quando uma versão mais recente é detectada, a atualização é obrigatória para continuar usando o aplicativo. A exigência é guardada no aparelho; é possível atualizar ou sair. O aplicativo confere a integridade e a assinatura do APK antes de pedir confirmação ao Android para instalar. Na edição para loja, esse atualizador está desativado e as atualizações são distribuídas pela loja. As políticas dos serviços e da loja também se aplicam.

## Apoio por Pix

A tela de apoio exibe dados de recebimento fornecidos pelo criador e permite copiar um código Pix ou visualizar um QR Code. A contribuição é voluntária. O aplicativo não acessa contas bancárias, não executa uma transferência, não recebe informações sobre a conta do contribuinte e não confirma que um pagamento ocorreu. A operação e o tratamento dos dados do pagamento acontecem no aplicativo e na instituição financeira escolhidos pelo usuário.

## Como apagar ou controlar dados

Use Sair da conta neste app para apagar a sessão técnica local. Limpar os dados do app ou desinstalá-lo remove os dados locais sob controle do aplicativo. Os arquivos da pasta Downloads e os cookies do navegador devem ser removidos nos respectivos aplicativos. Solicitações sobre dados tratados por Motorola/Lenovo, Google, GitHub, loja ou banco devem ser dirigidas aos respectivos responsáveis; o criador não controla os prazos de retenção desses serviços.

## Contato, público e alterações

Dúvidas sobre o aplicativo e solicitações relacionadas aos dados sob responsabilidade do criador podem ser encaminhadas ao contato informado acima. O aplicativo foi pensado para proprietários adultos de aparelhos e profissionais de assistência; não é direcionado a crianças. Alterações relevantes nesta política serão informadas na versão correspondente do aplicativo. Data desta revisão: 25 de novembro de 2026. Contato de suporte e privacidade: paradaseimportsoficial@gmail.com.

## Políticas e documentos dos serviços

- [Privacidade do Google](https://policies.google.com/privacy)
- [Privacidade Lenovo](https://www.lenovo.com/br/pt/privacy/)
- [Privacidade GitHub](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)



## Downloads retomáveis e relatórios locais

Novos downloads usam um serviço em primeiro plano com notificação e um arquivo parcial na coleção Downloads do Android, mantido pendente até a conclusão. A pausa preserva o parcial; cancelar o remove. O aplicativo guarda localmente o endereço temporário do arquivo, criptografado com Android Keystore, e metadados de progresso, tamanho e validação HTTP. Não guarda modelo ou IMEI para renovar automaticamente links. Um novo link pode ser consultado por ação do usuário; a retomada depende do suporte do servidor e da confirmação de identidade do arquivo. Após reiniciar o celular ou se o Android encerrar o serviço, abra o aplicativo para retomar. O Android pode limitar a duração do serviço. Ao concluir, o app verifica tamanho, CRCs do ZIP e calcula SHA-256; isso não comprova a origem ou autenticidade da ROM.

Os últimos 50 eventos técnicos permanecem locais e incluem horário, etapa, código fixo de erro, resposta HTTP, estado da rede, tentativas e progresso. O relatório preparado para e-mail também identifica a versão do app, do Android e o fabricante/modelo deste celular. Não inclui IMEI, credenciais, sessão, endereço completo de download ou conteúdo de respostas. Só é compartilhado se você escolher Reportar erro e enviar pelo seu aplicativo de e-mail após revisar. Limpar os dados do app remove os registros e o endereço criptografado; arquivos concluídos podem continuar em Downloads. Ao copiar o link ou abrir outro gerenciador, você compartilha com ele o endereço do firmware, que pode conter uma autorização temporária para esse arquivo. Nenhuma credencial da API é adicionada. O aplicativo externo aplica suas próprias políticas e controla o download.
