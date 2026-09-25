# Monitor EVO

Monitor de disponibilidade para computadores dedicados ao Controle de Acesso EVO.

## Instalar ou atualizar

[Baixar MonitorEVO.exe](https://github.com/mazzucahdw-prog/monitor-evo/releases/latest/download/MonitorEVO.exe)

1. Execute o arquivo e escolha **Instalar / atualizar**.
2. Confirme a instalação e a permissão do Windows. Configurar o controle antigo é opcional; o novo controle pode ser configurado depois no painel.
3. O painel abre após a instalação. O monitor permanece junto ao relógio do Windows.

Não é necessário desinstalar a versão anterior para atualizar no mesmo usuário. O instalador aproveita as configurações existentes. A execução com direitos de administrador vem selecionada quando a conta permite.

## Reabrir pelo menu Iniciar

A partir da 5.0.16, a instalação/atualização cria o atalho **Monitor EVO** no menu Iniciar do usuário. Pressione Windows e pesquise esse nome para abrir o painel. Se usou **Encerrar monitor**, clique em **Executar / retomar** para voltar às verificações.

O atalho é atualizado quando a versão muda e após restaurar a versão anterior. Não depende do instalador baixado na pasta Downloads. A desinstalação remove somente o atalho pertencente ao Monitor.

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

## Equipamentos de rede (5.0.12)

O módulo é opcional. Abra **Equipamentos de rede → Adicionar equipamento**. Cadastre um fabricante/modelo se necessário e selecione-o na lista. Informe um nome para o equipamento, IP esperado e a porta TCP realmente usada; marque **Ativar monitoramento**. É possível cadastrar até 32 dispositivos, com intervalo individual (padrão 30 segundos). O catálogo evita nomes duplicados por espaços, caixa e acentos.

O Monitor identifica automaticamente interfaces e máscaras IPv4 locais, tanto com IP fixo quanto DHCP. Verifica TCP, ping e, quando possível, MAC local. **Porta acessível** não significa catraca operando corretamente; **sem resposta** não comprova defeito físico ou causa na infraestrutura.

Para procurar um IP alterado, informe o MAC da etiqueta/configuração ou use **Usar MAC observado** após conferir uma leitura recente no IP esperado. Depois de três falhas, a busca automática pode procurar essa identidade nas redes locais. Ela não altera o endereço cadastrado nem configurações do Windows, EVO ou aparelho.

Use **Verificar / buscar agora** para solicitar uma nova leitura e **Cancelar busca** para interromper a procura. A pausa de manutenção também suspende o módulo. Novos resultados dependem do Monitor em execução; o painel informa quando as observações ficam antigas.

A busca usa até 256 endereços por interface e 1024 por rodada, quatro consultas simultâneas e cerca de 90 segundos. Sua repetição automática respeita 15 minutos por equipamento. Redes grandes e buscas que atingem limites são explicitamente parciais. ARP/MAC se aplica ao segmento local e não identifica equipamentos atrás de roteadores. Uma chamada do Windows já iniciada pode levar alguns segundos para concluir após o cancelamento.

O diagnóstico agora começa com **Resumo para suporte**, seguido dos detalhes técnicos. O painel ajusta os textos e permite rolar em janelas menores. A ajuda guiada e a integração com IA ficam para uma etapa futura.

As verificações desta entrega usaram redes/sondagens simuladas e telas renderizadas; ainda é necessária validação piloto com os equipamentos reais. O cadastro de equipamentos participa da recuperação de atualização.

## Inicialização do novo controle (5.0.30)

Em **Novo controle de acesso**, ajuste **Espera inicial após detectar o aplicativo**: padrão de **300 segundos (5 minutos)**, configurável de 0 a 300. Com o aplicativo monitorado, conta após encontrar o processo; reinicia a contagem se ele fechar ou reiniciar antes do fim. Sem monitorar o aplicativo, conta desde a primeira verificação. Zero remove só a espera extra.

Durante essa espera, o Monitor não abre nem age na página. Ela vale a cada início do Monitor, inclusive após atualização, e não se repete a cada reabertura da página. A presença do processo e o fim do prazo não comprovam saúde do serviço; uma página aberta pelo próprio aplicativo ou pelo Windows não é bloqueada.

Passe o mouse sobre as opções e tempos dessa tela para ler as explicações. A espera inicial é diferente da frequência de verificação, da primeira recarga e do retorno ao primeiro plano.

## Novas versões

A partir da **5.0.29**, o Monitor instalado consulta novas versões ao iniciar e instala em segundo plano, com as permissões de administrador que já possui. Não é necessário preencher novamente o formulário. A consulta e o download não pausam o monitoramento; a troca reinicia somente o Monitor e preserva as configurações.

Se a consulta, o download ou a validação falhar, a versão atual continua funcionando e a próxima tentativa ocorre após uma hora. Quando está atualizado, as consultas se repetem aproximadamente a cada seis horas. Durante manutenção, a instalação é adiada.

Se faltar permissão de administrador ou o Windows bloquear o atualizador independente, use **Verificar atualizações → Atualizar agora**. Não há pedido automático de elevação. Para receber a 5.0.29 a partir de uma versão anterior, use esse botão uma vez; o comportamento automático vale a partir da nova versão.

Se o novo agente não confirmar sua inicialização, o instalador tenta restaurar a versão anterior. Uma versão revertida ou com instalação automática incerta fica bloqueada para reinstalação automática do mesmo pacote. Uma versão posterior pode ser instalada; uma nova tentativa manual continua disponível. Essa verificação não detecta toda regressão funcional: **Restaurar versão anterior** permanece disponível no painel.

A correção específica de tela cheia por F11 ainda está em validação e não está incluída na 5.0.29. O modo quiosque/privado não foi reintroduzido.

O navegador pode avisar que o arquivo é pouco baixado. Este protótipo ainda não possui assinatura Authenticode de um publicador reconhecido. A assinatura do registro de atualização não elimina avisos de reputação do navegador ou do Windows.

O registro de atualização usa assinatura RSA-SHA256 e inclui a verificação SHA-256 do instalador. Essa assinatura de atualização não substitui a assinatura Authenticode/reputação do executável no Windows.

## Piloto de atualização

As versões 5.0.7 e 5.0.8 são uma entrega piloto para validar o fluxo. Para testar a detecção, instale a [5.0.7](https://github.com/mazzucahdw-prog/monitor-evo/releases/download/v5.0.7/MonitorEVO.exe), abra **Verificar atualizações** e confira a oferta da versão mais recente.

Os testes automatizados incluem simulações de instalação e recuperação, assinatura inválida, arquivo alterado e download incompleto. Não representam validação da instalação com UAC nem da recuperação em um computador cliente real.

## Publicação

Este repositório distribui o aplicativo e as notas de versão. Credenciais, dados de clientes e chaves privadas não fazem parte da distribuição.
