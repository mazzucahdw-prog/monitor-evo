# Monitor EVO

Monitor de disponibilidade para computadores dedicados ao Controle de Acesso EVO.

## Instalar ou atualizar

[Baixar MonitorEVO.exe](https://github.com/mazzucahdw-prog/monitor-evo/releases/latest/download/MonitorEVO.exe)

1. Execute o arquivo e escolha **Instalar / atualizar**.
2. Confira o atalho do EVO e confirme a instalação e a permissão do Windows.
3. O painel abre após a instalação. O monitor permanece junto ao relógio do Windows.

Não é necessário desinstalar a versão anterior para atualizar no mesmo usuário. O instalador aproveita as configurações existentes. A execução com direitos de administrador vem selecionada quando a conta permite.

## Verificação e ajuda ao cliente

Na versão 5.0.10, use **Configurações → Verificar EVO a cada (segundos)** para escolher de 1 a 30 segundos. O padrão é 5 segundos. Na atualização de versões anteriores, o antigo padrão de 2 segundos passa a 5; outros intervalos personalizados são preservados. Os prazos de reabertura e recuperação de foco são configurações separadas.

O painel distingue **Monitor ativo às** de **Última verificação do EVO**. Durante a pausa, o Monitor confirma que está ativo, mas a verificação do EVO fica suspensa.

O botão **Preciso de ajuda** mostra orientações conforme o resultado atual, com atalhos para conferir a configuração, retomar o monitoramento, recuperar a janela ou preparar um diagnóstico. Uma abertura em andamento não gera uma nova tentativa pela ajuda. As observações do processo do EVO não comprovam o funcionamento da catraca ou da rede.

## Aplicativos adicionais e manutenção (5.0.11)

Use **Aplicativos adicionais → Adicionar** para cadastrar até oito aplicativos além do EVO. Escolha o arquivo; o processo é preenchido quando identificado. Informe um nome e marque **Ativar monitoramento**. A opção **Reabrir automaticamente se estiver fechado** é separada e começa desmarcada. Cada aplicativo tem seu intervalo e prazo de reabertura. Os adicionais não tomam o foco do EVO nem são encerrados automaticamente.

O arquivo escolhido é comparado à identidade do processo configurado. Atalhos incompatíveis ou sem identidade verificável geram aviso e não são abertos pelo Monitor. Essa conferência evita escolhas erradas; não substitui uma assinatura de publicador.

Em **Pausa de manutenção**, escolha de 1 a 1440 minutos ou **Sem prazo**. O padrão é 15 minutos e pode ser salvo. Aplicar novamente começa o prazo a partir daquele momento. **Retomar agora** encerra a pausa de todos os aplicativos monitorados.

## Recuperação de atualização

A atualização guarda os arquivos anteriores e as configurações. Falhas da transação de instalação acionam a recuperação automática. Se perceber uma regressão depois, use **Restaurar versão anterior** e confirme a permissão do Windows. A versão anterior é conferida por integridade antes da troca; suas configurações anteriores também são restauradas. Alterações feitas após a atualização podem ser desfeitas.

Essa opção precisa de uma instalação anterior registrada neste computador. Não há detecção automática de toda regressão funcional. Os testes de recuperação foram isolados e simulados; a validação em computador cliente faz parte do piloto.

## Novas versões

A partir da versão 5.0.7, o Monitor consulta este repositório automaticamente, aproximadamente a cada seis horas. Você pode usar **Verificar atualizações** no painel ou no menu junto ao relógio.

Quando houver uma versão nova, o painel destaca a atualização. Escolha **Atualizar agora** para baixar o pacote verificado e abrir o instalador. A instalação ainda requer a confirmação normal do Windows. **Mais tarde / fechar** mantém a versão atual funcionando.

A partir da 5.0.9, uma instalação existente é atualizada sem repetir a seleção do atalho ou de direitos de administrador. O Monitor reutiliza as configurações e permissões salvas. A primeira instalação continua mostrando a configuração inicial. A confirmação de administrador do Windows ainda pode aparecer.

O navegador pode avisar que o arquivo é pouco baixado. Este protótipo ainda não possui assinatura Authenticode de um publicador reconhecido. A assinatura do registro de atualização não elimina avisos de reputação do navegador ou do Windows.

O registro de atualização usa assinatura RSA-SHA256 e inclui a verificação SHA-256 do instalador. Essa assinatura de atualização não substitui a assinatura Authenticode/reputação do executável no Windows.

## Piloto de atualização

As versões 5.0.7 e 5.0.8 são uma entrega piloto para validar o fluxo. Para testar a detecção, instale a [5.0.7](https://github.com/mazzucahdw-prog/monitor-evo/releases/download/v5.0.7/MonitorEVO.exe), abra **Verificar atualizações** e confira a oferta da versão mais recente.

Os testes automatizados incluem simulações de instalação e recuperação, assinatura inválida, arquivo alterado e download incompleto. Não representam validação da instalação com UAC nem da recuperação em um computador cliente real.

## Publicação

Este repositório distribui o aplicativo e as notas de versão. Credenciais, dados de clientes e chaves privadas não fazem parte da distribuição.
