# Segurança e autenticidade

## Download oficial

Baixe o ROMFlow em https://github.com/paradaseimportsoficial-ops/ROMFlow/releases/latest.
Prefira compartilhar esse link em vez de repassar cópias do APK.

O SHA-256 do arquivo consta em `SHA256SUMS.txt`, na mesma release. Ele identifica
os bytes daquela versão; não é o mesmo que a impressão digital do certificado.

Impressão digital SHA-256 do certificado oficial da distribuição direta:

```
9D:30:21:8C:B2:60:B0:83:41:76:AF:31:81:8E:19:94:7F:A6:E3:BA:2F:2D:BF:96:E3:4C:A3:65:0D:07:D8:2C
```

Essa impressão digital é pública e não contém a chave privada de assinatura.
Copiar seu texto não permite assinar um APK como o autor.

Para conferir no computador, com as ferramentas oficiais Android SDK Build Tools:

```
apksigner verify --verbose --print-certs ROMFlow.apk
```

Compare o SHA-256 do certificado exibido com o valor acima e confira o hash do
arquivo com `SHA256SUMS.txt`. Uma cópia encontrada em outro site não é uma fonte
oficial; somente o endereço de origem ou o nome do arquivo não comprovam autoria.
Hashes publicados no mesmo local não substituem a proteção da conta do publicador.

## Relatar um problema

Use **Report a vulnerability** na aba Security para um relato privado, ou envie para
**paradaseimportsoficial@gmail.com**. Informe versão, Android, passos para
reproduzir e impacto observado. Não envie senhas, tokens de sessão, IMEI completo,
chaves privadas ou dados de clientes. Remova esses dados de capturas e logs.

O recebimento será analisado conforme a disponibilidade do mantenedor; não há
prazo ou recompensa garantidos. Combine a divulgação responsável antes de
publicar detalhes que exponham usuários. Para bugs comuns, use as Issues sem
informações pessoais. Prefira a versão mais recente; versões antigas não têm
suporte de manutenção garantido.

O projeto Android não está neste repositório público. Os arquivos automáticos
“Source code” das releases contêm os materiais públicos do repositório. A licença
não é uma barreira técnica contra análise de APKs nem impede implementações
independentes das mesmas funcionalidades.

## Versões e limites de proteção

A versão de manutenção atual é a 0.1.23. Prefira a release mais recente. O aplicativo usa assinatura de produção, verificações de integridade e validação do APK de atualização. Isso não torna um APK impossível de analisar ou modificar: confira o certificado e use a distribuição oficial.

SH gerado pelo ROMFlow é importado como um plano fechado, com correspondência integral ao gerador e verificação dos arquivos; o app não executa Bash arbitrário. Um plano reconhecido ou um checksum correto não comprova a autenticidade da ROM nem sua compatibilidade com downgrade. A revisão final distingue comandos executados de etapas omitidas no modo escolhido.

Relatórios técnicos são locais e só saem pelo aplicativo de e-mail após revisão e envio do usuário. Não publique links completos de sessão ou download temporário.
