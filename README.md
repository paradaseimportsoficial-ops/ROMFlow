# ROMFlow — ROMs Motorola e ferramentas USB

<img src="docs/icone-512.png" width="96" alt="Ícone do ROMFlow">

**Aplicativo Android para consultar e baixar firmware original Motorola e realizar instalações e operações compatíveis em outro aparelho por USB/OTG, sem computador.**

Por **Técnico Root — Ivanildo Sousa**. Projeto independente, sem vínculo com Motorola ou Lenovo.

## Download

**[📥 Baixar a versão mais recente](https://github.com/paradaseimportsoficial-ops/ROMFlow/releases/latest)**

Baixe **ROMFlow.apk** na publicação mais recente. O arquivo **SHA256SUMS.txt** permite conferir o download. A versão **0.1.23** melhora downloads, diagnóstico e o fluxo de instaladores. Português, inglês, espanhol e árabe continuam disponíveis. Instale por cima da versão anterior para manter os dados do aplicativo.

## Funções

- **Idiomas:** português (Brasil), inglês, espanhol e árabe, com troca pelo botão 🌐 Idioma na tela principal.
- **Baixar ROM:** catálogo Motorola/Lenovo, consulta por modelo XT e IMEI e download no celular.
- **Meus downloads:** pausa e retomada, progresso, velocidade e estimativa de tempo; preserva o arquivo parcial quando possível. A retomada depende do servidor e da identidade do arquivo.
- **Download externo:** copiar o link temporário ou abrir em navegador/gerenciador compatível, sem compartilhar credenciais da API.
- **Modelo automático sem root:** confira a sugestão do modelo e informe o IMEI manualmente.
- **Reconhecimento USB:** identifica outro Motorola em fastboot por USB/OTG quando o aparelho fornece os dados.
- **Instalar ROM:** confere imagens e prepara firmware original compatível para outro Motorola, com escolha entre instalação limpa e tentar manter dados, revisão do plano final e das etapas omitidas.
- **Converter XML em SH:** exporta `flash-romflow.sh` para Bash/Termux e permite importar o SH gerado pelo próprio ROMFlow, por formato fechado e verificações SHA-256. SHs novos não precisam do XML separado; scripts antigos da beta.4 exigem o XML correspondente.
- **Diagnóstico:** eventos locais e relatório técnico para revisar e enviar voluntariamente pelo seu aplicativo de e-mail, sem IMEI ou credenciais no relatório.
- **Avançado:** flash de imagens, seleção de slot A/B ou ambos, boot temporário, ZIP por ADB sideload e instaladores BAT/SH/XML compatíveis.

As operações avançadas também podem ser usadas com custom ROMs e recoveries compatíveis. Siga o guia específico do aparelho e do pacote; não há suporte universal a qualquer celular ou script.

## Como usar

É necessário Android 10 ou superior, internet e espaço livre. Para consultar o catálogo, entre na conta Motorola/Lenovo, confira o modelo e informe o IMEI. A ajuda do aplicativo mostra onde encontrar esses dados nas configurações ou com `*#06#` no app Telefone.

Para operações USB, use um celular controlador com USB Host/OTG, cabo compatível e outro aparelho no modo indicado pelo guia da ROM. **O ROMFlow não instala a ROM no próprio celular em que está aberto.**

A consulta manual e as funções USB não exigem root. A edição do GitHub oferece **Ler este celular com root** na tela de consulta, como alternativa opcional. O IMEI pode continuar indisponível mesmo com autorização; complete manualmente nesse caso.

## Downloads e instaladores

Pausar preserva o parcial. Após reiniciar o celular ou se o Android encerrar o serviço, abra Meus downloads para retomar. Se o link expirar, consulte a mesma ROM novamente; o app só reutiliza o parcial quando consegue confirmar a identidade do arquivo. CRC e checksum verificam corrupção, mas não comprovam autenticidade de um pacote importado. Use fontes confiáveis.

Ao importar, selecione a pasta que contém o instalador e suas imagens, mantendo as subpastas exigidas. A tela mostra o nome e o formato selecionados, depois confere os arquivos. BAT/SH externos têm suporte restrito a comandos reconhecidos; não há execução livre de shell. O perfil Stomo mantém suas exigências próprias e pode precisar de formatação manual pelo recovery.

## Antes de gravar

Faça backup e confirme modelo, variante e ROM. Arquivos ou partições incorretos podem apagar dados ou impedir a inicialização. Tentar manter dados não garante sua preservação. O aplicativo não desbloqueia nem bloqueia o bootloader.

Gravar ambos os slots sobrescreve as duas cópias; não muda o slot ativo nem duplica uma ROM inteira automaticamente. Use o modo adequado do aparelho para cada partição. Revise todas as etapas e apagamentos do instalador e conclua a formatação manual no recovery quando o fluxo exigir. ZIP de recovery não deve ser tratado como imagem de partição.

O mantenedor validou instalação stock por XML usando Edge 50 Fusion como controlador e Moto G84 como destino, mantendo dados, e aprovou os fluxos SH/XML nas betas da 0.1.23. **BAT ainda não teve teste físico nesta atualização.** Há testes automatizados, inclusive Bash com fastboot simulado; eles não comprovam compatibilidade universal ou substituem teste no aparelho.

## Interface

Captura da versão 0.1.16; detalhes podem diferir da versão atual.

<img src="docs/capturas/inicio-016.png" width="300" alt="Tela inicial do ROMFlow">

## Histórico das atualizações

| Versão | Resumo |
| --- | --- |
| 0.1.23 | Downloads retomáveis, links externos, diagnóstico, conversão/importação SH, revisão de instaladores e traduções da licença. |
| 0.1.22 | Português, inglês, espanhol e árabe, com seletor de idioma. |
| 0.1.21 | Atualização de segurança. |
| 0.1.20 | Atualização de segurança. |
| 0.1.19 | Manutenção da interface. |
| 0.1.18 | Seleção de slots A/B no flash avulso e ajustes de navegação. |
| 0.1.17 | Sugestão automática do modelo sem root. |
| 0.1.16 | Operações USB avançadas e importação de instaladores compatíveis. |
| 0.1.15 | Identificação de outro Motorola por fastboot USB/OTG. |
| 0.1.14 | Preparação e instalação de ROM original por USB/OTG. |
| 0.1.13 | Atualização da apresentação do apoio por Pix. |
| 0.1.12 | Atualização da marca Técnico Root. |
| 0.1.11 | Publicidade e diagnóstico. |
| 0.1.10 | Padronização do nome ROMFlow e da pasta de downloads. |
| 0.1.9 | Consulta e download de firmware Motorola. |

As páginas das releases preservam as notas das versões. Prefira sempre o APK mais recente. Os links automáticos **Source code** do GitHub são cópias dos materiais deste repositório público: **não contêm o projeto Android do aplicativo**.

## Privacidade e suporte

O app contém anúncios e oferece apoio voluntário por Pix. Anúncios dependem da disponibilidade e autorização do AdMob; a ausência de um anúncio não impede o acesso ao arquivo baixado. Leia a [política de privacidade](docs/PRIVACIDADE.md).

Contato: [paradaseimportsoficial@gmail.com](mailto:paradaseimportsoficial@gmail.com). Ao relatar problemas, informe a versão do app, o Android e o que aconteceu. Não publique IMEI, credenciais ou links de sessão.

## Créditos

Base técnica adaptada de [Moto Firmware Downloader, de JoshRob](https://github.com/JoshRob297/moto-firmware-downloader), sob [licença MIT](THIRD_PARTY_LICENSES.txt). Marcas pertencem aos respectivos titulares.

Este repositório público reúne a distribuição e a documentação de uso.


## Licença e autenticidade

As contribuições originais do ROMFlow seguem os termos da [licença do aplicativo](LICENSE). Os componentes de terceiros mantêm suas próprias permissões e créditos em [THIRD_PARTY_LICENSES.txt](THIRD_PARTY_LICENSES.txt). A licença MIT da base de JoshRob não se aplica automaticamente a todas as contribuições originais do ROMFlow.

Consulte [Segurança e autenticidade](SECURITY.md) para conferir o certificado oficial e relatar vulnerabilidades em particular.


Certificado oficial SHA-256 da distribuição direta:

```text
9D:30:21:8C:B2:60:B0:83:41:76:AF:31:81:8E:19:94:7F:A6:E3:BA:2F:2D:BF:96:E3:4C:A3:65:0D:07:D8:2C
```

Com Android SDK Build Tools, confira com `apksigner verify --verbose --print-certs ROMFlow.apk` e compare o certificado com o valor acima. Confira também o hash do arquivo em `SHA256SUMS.txt`. A impressão digital é pública; não contém a chave privada.
